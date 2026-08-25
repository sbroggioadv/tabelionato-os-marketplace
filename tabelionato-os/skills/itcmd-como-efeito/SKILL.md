---
name: itcmd-como-efeito
description: "Trata o ITCMD e tributos conexos como efeitos e gates documentais dos atos notariais, sem lançar, arrecadar, calcular alíquota ou transportar legislação entre UFs, aplicando Resolução CNJ 35/2007 e normas gerais da LC 227/2026. Esta skill deve ser usada quando o pedido mencionar ITCMD, imposto de transmissão, inventário, doação, partilha desigual, renúncia de herança, multa por atraso, guia fiscal, fato gerador, alíquota estadual ou tributo antes da lavratura."
---

# ITCMD como efeito

> Camada C5. O tabelião verifica o gate tributário do ato; não constitui nem arrecada o crédito tributário.

## Anexos e skills obrigatórios

- `context/res-cnj-35-2007-com-571-2024.md` — arts. 15, 22, 31, 38 e 11-A;
- `context/travas-defasagem.md` — travas T-84 e T-85;
- `context/emolumentos-norma-por-uf.md` — proibição de transportar regras estaduais;
- `context/sequencia-do-ato.md` — tributo antes da lavratura e distinção de emolumentos;
- `roteador-uf`, `primeira-etapa-e-onde-entram-as-custas`, `emolumentos-norma-da-uf` e `qualificacao-notarial-transversal`.

## Entradas bloqueantes

Confirmar UF, município quando outro tributo puder incidir, data do fato gerador, espécie do ato, transmissão envolvida, bens e localização, quinhões ou frações, domicílios relevantes, existência de renúncia, aceitação anterior, guias, comprovantes, certidão fiscal e multa. Não presumir incidência, isenção, base ou alíquota.

## Papel do tabelião

Nos atos submetidos à Resolução CNJ 35/2007:

- exigir que o recolhimento dos tributos incidentes anteceda a lavratura, conforme art. 15;
- conferir a documentação fiscal prevista no art. 22;
- permitir a escritura a qualquer tempo, mas fiscalizar eventual multa por atraso conforme a lei estadual ou distrital, nos termos do art. 31;
- documentar guias e respectivos valores na autorização de alienação do art. 11-A;
- em transmissão entre cônjuges ou partilha desigual, exigir prova do tributo somente sobre a fração transferida, conforme art. 38.

Classificar a falta de recolhimento prévio, quando exigido, como trava impeditiva condicional. Não confundir esse gate com emolumento nem dizer que custas são o primeiro passo do atendimento.

## Normas gerais da LC 227/2026

Usar a LC 227/2026 como camada nacional de normas gerais, não como tabela estadual:

- reconhecer fatos geradores distintos por sucessor ou donatário e ente competente;
- lembrar que o fato gerador causa mortis independe da abertura de inventário judicial ou extrajudicial;
- aplicar a alíquota vigente na abertura da sucessão para causa mortis e na doação para doação;
- tratar progressividade por faixas conforme a lei aplicável;
- identificar sucessor ou donatário como contribuinte conforme a hipótese;
- para imóvel no Brasil, localizar a competência no Estado ou DF da situação do bem, mesmo com pessoa no exterior.

Não informar percentual, valor, teto ou benefício sem confirmar a legislação vigente da UF na data relevante.

## Renúncia

Tratar como não incidência apenas a renúncia cumulativamente:

1. sem ressalva ou condição;
2. em benefício do monte;
3. sem ato anterior que demonstre aceitação.

Se houver beneficiário determinado, condição, ressalva ou aceitação anterior, não chamar automaticamente de renúncia abdicativa. Classificar a possível transmissão e exigir análise tributária da UF, sem concluir por memória que é doação.

## Separar efeitos

Distinguir ITCMD, ITBI, imposto de renda, multa, emolumentos, fundos, selo e despesas. Cada parcela tem competência, fato gerador e momento próprios. Não transportar alíquota, isenção, guia, prazo ou sanção de uma UF para outra.

## Saída

Entregar matriz por transmissão e beneficiário, ente competente, data do fato gerador, documentos fiscais, gate antes da lavratura, multa, fração transferida, estado da renúncia e pendências estaduais. Exibir valores apenas quando vierem de documento do caso e identificá-los como dado, nunca como cálculo próprio.

## Reprovação automática

- lançar, arrecadar ou calcular ITCMD;
- informar alíquota ou isenção sem UF, data e norma;
- dizer que o imposto nasce com a abertura do inventário;
- tributar toda a partilha quando só há fração transferida;
- tratar toda renúncia como não incidência;
- ignorar aceitação anterior;
- confundir tributo com emolumento;
- transportar regime de outra UF.
