---
name: duvida-notarial-por-uf
description: "Classifica a dúvida notarial na taxonomia canônica A1, A2, A3, B e C das 27 UFs, separando rito geral, hipótese restrita, intervenção em dúvida registral alheia e cobertura parcial. Esta skill deve ser usada quando o pedido mencionar suscitar dúvida, dúvida inversa, recusa contestada, levar a negativa ao juízo, obrigação do tabelião, intervenção em dúvida registral, nota devolutiva ou caminho do interessado após a qualificação negativa."
---

# Dúvida notarial por UF

> Camada C2. Classificar antes de orientar. A Lei de Registros Públicos não cria, por si só, rito geral de dúvida para o tabelião de notas.

## Anexos obrigatórios

- `context/uf-matriz-27.md` — matriz derivada da fonte canônica A1/A2/A3/B/C;
- `context/sequencia-do-ato.md` — fronteira entre nota, dúvida e encaminhamento;
- `context/travas-defasagem.md` — iscas registrais e armadilhas de destinatário;
- `context/estado-da-norma.md` — redação vigente na data de corte.

## Entrada bloqueante

Fixar UF, ato, fundamento da recusa, requerimento do interessado e fase do procedimento. Sem UF, não prometer suscitação: o esqueleto federal não contém protocolo, prazo ou nota de exigências para Notas, e o rito dos arts. 198 e seguintes da Lei 6.015/1973 é registral salvo extensão estadual comprovada.

## Taxonomia canônica

Aplicar exatamente:

- **A1 — 8 UFs:** PI, PA, TO, CE, MG, PB, RR e MA. Há nota/exigência dirigida ao tabelião e dúvida; RR remete a “prazo legal” sem número, e MA a “prazos normativos respectivos”.
- **A2 — 6 UFs:** AP, MS, RN, SC, RJ e ES. Há dúvida notarial expressa, mas não prazo geral de análise dirigido ao tabelião; no AP, registrar a assimetria do art. 231.
- **A3 — 3 UFs:** AL, DF e MT. Há somente hipótese restrita ou remissão: AL remete à sistemática federal; DF limita ao inventário/partilha com testamento; MT limita à divergência de valor declarado.
- **B — 9 UFs:** AC, AM, BA, GO, PE, PR, RS, SE e SP. Há dever ou regra de recusa, mas não rito geral próprio de dúvida notarial. BA e RS apenas admitem intervenção do tabelião em dúvida registral alheia; isso não cria suscitação própria.
- **C — 1 UF:** RO. Foi localizado rito registral, não recusa/dúvida notarial geral; manter a cobertura parcial.

Preservar os três números sem fundi-los: **17 UFs** estão na Categoria A; somente **14** possuem dúvida notarial geral de A1+A2; somente **8** possuem prazo ou nota dirigida ao tabelião; somente **6** fixam número de prazo — PI, PA, TO, CE, MG e PB.

## Algoritmo

### 1. Confirmar o destinatário

Ler o dispositivo no documento-mãe e procurar menção a tabelião, notário ou todas as atribuições. Rejeitar artigo de Registro de Imóveis, Protesto, RTD ou RCPJ usado apenas porque contém “dúvida”, “nota devolutiva” ou “tabelião”.

### 2. Aplicar o alcance da categoria

- Em **A1**, coordenar nota, prazo local e suscitação; acionar `prazos-e-protocolo-por-uf`.
- Em **A2**, formalizar a negativa conforme a UF e orientar o rito sem inventar prazo de análise. No RJ, preservar os cinco dias do interessado.
- Em **A3**, testar primeiro a hipótese fechada. Fora dela, declarar inexistência de rito próprio geral.
- Em **B**, não prometer que o interessado pode obrigar o tabelião a suscitar dúvida geral. Indicar reclamação, pedido de providências ou via correcional somente quando localizada.
- Em **C**, rotear para a DGE e declarar a insuficiência específica.

### 3. Tratar dúvida inversa e inércia

Aplicar somente o desenho da UF. Distinguir petição direta ao juízo, protocolo por intermédio do delegatário, prazo de inércia, preservação da prenotação e legitimidade recursal. Não importar o desenho de PA, PB, AP, MA ou RN para outro estado.

### 4. Evitar falsos positivos

- Não usar regra de Protesto do PR ou de GO como rito de Notas.
- Não contornar a exclusão expressa de Notas no AM.
- Não transformar a intervenção de BA ou RS na dúvida registral em rito próprio notarial.
- Não tratar o art. 178 da DGE/RO como recusa notarial geral.
- Não converter precedente ou consulta correcional em autorização para transferir a qualificação.

## Saída

| Campo | Resultado |
|---|---|
| UF, ato e data de corte | |
| categoria | A1, A2, A3, B ou C |
| alcance | geral, restrito, ausente ou parcial |
| nota/recusa anterior | forma e fundamento |
| legitimado e iniciativa | |
| prazo e marco | somente se localizados |
| destino e documentos | |
| dúvida inversa | desenho local ou ausência |
| lacunas | |

## Reprovação automática

- alterar qualquer lista ou total da taxonomia;
- prometer rito geral em A3, B ou C;
- afirmar prazo de análise em A2;
- dizer que as 17 UFs da Categoria A possuem rito geral;
- usar dispositivo registral sem extensão expressa a Notas;
- omitir a assimetria do AP ou a cobertura parcial de RO;
- apresentar intervenção alheia como poder de suscitação própria.
