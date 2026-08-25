---
name: roteador-uf
description: "Motor estadual de triagem: resolve documento-mãe, autoridade competente, forma de citação, contagem de prazo, regime de IA, rito notarial e arquitetura de emolumentos a partir da UF, sem reproduzir a matriz completa. Esta skill deve ser usada quando o pedido mencionar qual norma estadual vale, qual corregedoria rege a serventia, trocar ou declarar UF, Código de Normas, prazo estadual, recusa, dúvida, IA ou emolumentos por estado."
---

# Roteador UF

> Camada C2. Fixar a UF antes de qualquer afirmação estadual. Não transportar regra entre unidades federativas.

## Anexos obrigatórios

Abrir, nesta ordem:

1. `context/estado-da-norma.md` — data de corte, vigência e alteradores;
2. `context/uf-matriz-27.md` — matriz-mestra das 27 UFs;
3. `context/travas-defasagem.md` — armadilhas de destinatário, citação e consolidação.

Carregar o anexo temático somente depois do roteamento. Manter a matriz de 27 UFs no anexo; não copiá-la para a resposta nem para esta skill.

## Entrada bloqueante

Exigir sigla ou nome inequívoco da UF. Normalizar apenas equivalências seguras, como `Piauí` → `PI`; não deduzir UF por município, tribunal, nome de parte, IP, metadado ou conteúdo de documento.

Quando a UF estiver ausente:

1. rotular a resposta como **esqueleto federal**;
2. limitar a resposta às normas federais efetivamente aplicáveis;
3. declarar literalmente: **“O esqueleto federal não tem protocolo, prazo nem nota de exigências para o tabelionato de notas.”**;
4. não afirmar rito de dúvida notarial, forma de recusa, contagem, autoridade estadual, norma estadual de IA ou tabela de emolumentos;
5. solicitar a UF antes de prosseguir no bloco estadual.

## Algoritmo de roteamento

### 1. Localizar a linha da UF

Ler uma única linha de `uf-matriz-27.md` e extrair:

- documento-mãe e ato instituidor;
- autoridade correcional competente;
- endereço e situação da norma estadual de IA;
- estado da cobertura disciplinar;
- categoria A1, A2, A3, B ou C do rito notarial;
- lei, índice, ato e anomalias de emolumentos;
- forma de citação e regra de contagem de prazo.

Não completar campo ausente por analogia com UF vizinha. Distinguir **não localizado**, **não fixado**, **remetido sem número** e **não aplicável**.

### 2. Resolver documento e autoridade

Reproduzir o nome real do documento. Aplicar as exceções de identidade:

- chamar o documento de RO de **DGE**;
- chamar o documento de TO de **Consolidação**;
- usar **CFE** no PI, **COGEX** no MA, BA e GO, e **CGFE** em SC;
- preservar no PA o órgão do ato-mãe — CJRMB/CJCI — e distinguir os alteradores CGJ;
- não converter essas autoridades em “CGJ do estado”.

Preservar também a gramática de citação: quatro dígitos no AP; título e artigo em AL; número com ano em GO; capítulo e item em SP; sigla emissora integral em TO; corpo, e não sumário, na PB.

### 3. Rotear o assunto

Acionar:

- `regime-de-ia-da-uf` para autorização, vedação, contratação, homologação ou governança de IA;
- `recusa-e-nota-de-exigencias-por-uf` para forma, fundamentos e conteúdo da recusa/exigência;
- `duvida-notarial-por-uf` para suscitação, alcance geral ou hipótese restrita;
- `prazos-e-protocolo-por-uf` para protocolo, marco inicial, unidade e assinatura;
- `emolumentos-norma-da-uf` para lei, índice, ato, tabela e parcelas externas.

Executar mais de uma skill quando o caso cruzar blocos. Não deixar um achado de um bloco preencher a lacuna de outro.

### 4. Aplicar cobertura honesta

- Tratar 26 UFs como cobertas nos blocos indicados pela matriz.
- Tratar RO como parcial: rotear para a DGE, declarar o ponto não capturado e não inventar PAD, recusa notarial ou norma-mãe de emolumentos.
- Tratar ausência expressa como resultado, não como convite à suposição.
- Conferir `estado-da-norma.md` antes de apresentar qualquer endereço como vigente.

## Cartão de saída

Entregar sem valores ou dados pessoais:

| Campo | Resultado |
|---|---|
| UF e data de corte | |
| documento-mãe e ato | |
| autoridade competente | |
| forma de citação | |
| IA estadual | norma, ausência ou bloqueio |
| rito notarial | A1, A2, A3, B ou C |
| contagem de prazo | regra localizada ou lacuna |
| emolumentos | lei/índice/ato, sem quantia |
| skill seguinte | |
| lacunas | |

## Reprovação automática

- responder bloco estadual sem UF;
- chamar todo documento de “Código de Normas da CGJ”;
- confundir inexistência de norma estadual de IA com autorização ou proibição;
- atribuir protocolo, prazo ou nota ao piso federal;
- transportar regime, prazo, rito, autoridade ou tabela de outra UF;
- esconder a cobertura parcial de RO;
- reproduzir as 27 linhas da matriz dentro da skill ou da resposta sem necessidade.
