---
name: perfil-da-serventia
description: "Memória institucional mínima do tabelionato-os. Persiste e fornece ao motor UF-aware somente UF, classe TIC, atribuições, estágio de uso de IA, situação da delegação e data de corte do contexto, sem acervo nem dados pessoais. Esta skill deve ser usada ao concluir ou atualizar o onboarding, antes de rotear norma estadual, ao retomar uma sessão, quando outra skill precisar da UF/classe/perfil, ou quando o pedido mencionar perfil da serventia, memória, onde paramos, atualizar configuração, apagar perfil ou data de corte."
---

# Perfil da Serventia — estado institucional

> Camada C0. Guardar apenas o que evita repetir o onboarding e permite roteamento normativo. Não funcionar como memória de caso.

## Objetivo e ativação

Criar, ler, atualizar, invalidar ou apagar o perfil institucional. Ativar ao concluir `tabelionato-onboarding`, no início de `tabelionato-master`, quando o motor estadual precisar de UF/classe ou quando a data de corte mudar.

## Esquema permitido

```yaml
schema_version: 1
uf: XX
classe_tic: classe_1 | classe_2 | classe_3 | nao_confirmada
atribuicoes:
  modelo: notas_isolado | oficio_unico | acumulada | nao_confirmada
  categorias: []
uso_ia: nao_usa | avaliacao | piloto | producao | nao_confirmado
situacao_delegacao: provida | vaga_interino | transicao | nao_confirmada
data_corte_contexto: 25/08/2026
atualizado_em: AAAA-MM-DD
```

Manter `categorias` em vocabulário institucional, como `registro_imoveis`, `registro_civil`, `protesto` ou `outra_atribuicao`; não guardar número, pessoa ou localização detalhada.

## Operações

### Criar

1. Receber a ficha confirmada do onboarding.
2. Validar UF contra as 27 siglas.
3. Validar enums e data de corte.
4. Persistir o perfil em área de estado do workspace definida pelo host.
5. Confirmar somente os campos institucionais.

### Ler

1. Carregar antes do roteamento estadual.
2. Informar campos ausentes como `nao_confirmada`; não inferir.
3. Comparar `data_corte_contexto` com `context/estado-da-norma.md`.
4. Acionar onboarding se o perfil estiver ausente ou incompatível com o esquema.

### Atualizar

1. Alterar somente campos confirmados pelo operador.
2. Preservar os demais.
3. Atualizar o marco temporal.
4. Reexecutar gates dependentes quando UF, classe, IA ou situação da delegação mudar.

### Invalidar

Marcar a base como defasada quando a data do perfil divergir do contexto ou o gate de vigência detectar alteração posterior. Manter o perfil institucional, mas bloquear afirmação de vigência atual até atualizar os anexos.

### Apagar

Atender pedido explícito de exclusão do perfil. Confirmar o alvo exato e apagar somente o registro institucional, sem tocar documentos do workspace.

## Consumidores do perfil

- `tabelionato-master`: evita perguntar novamente a UF e dispara o fluxo correto;
- motor UF-aware: lê UF, órgão, rito, prazos e emolumentos;
- camada de IA: lê UF, estágio e situação provida/interina;
- camada de acervo/TIC: lê classe;
- `suprema-corte-tabelionato`: compara UF e data de corte.

Nenhuma skill deve tratar o perfil como prova de fato de um ato. Confirmar novamente modalidade, competência, partes, documentos e circunstâncias a cada demanda.

## Dados proibidos

Não guardar:

- nome, CPF/CNPJ, e-mail, telefone, endereço ou matrícula de pessoa;
- número da serventia, delegação, processo, protocolo, selo ou ato;
- parte, cliente, advogado, escrevente ou fornecedor identificado;
- documento, minuta, livro, imagem, prompt, log ou conteúdo de acervo;
- receita exata, emolumento, contrato ou credencial.

## Entrega obrigatória

Ao ler ou atualizar, devolver ficha concisa, campos não confirmados, data de corte e efeito no roteamento. Não expor caminho interno de armazenamento nem conteúdo além do esquema.

## Guard

Aplicar minimização. Dado não necessário ao roteamento não entra. Se outra skill tentar persistir informação de caso ou acervo, recusar a gravação e manter apenas a categoria institucional permitida.
