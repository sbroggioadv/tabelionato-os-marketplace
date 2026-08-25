---
name: varredura-de-vigencia-pre-lavratura
description: "Gate pré-lavratura que verifica situação do provimento, redação vigente do dispositivo no consolidado, norma da corregedoria estadual e tipo do ato, sempre com fonte e data de corte. Exibe o estado normativo e devolve a decisão ao titular. Esta skill deve ser usada antes de afirmar que uma norma está vigente ou antes de minuta/lavratura, ou quando o pedido mencionar conferir vigência, norma atual, artigo superado, atualização da CGJ, checagem prévia, gate normativo, posso usar este provimento ou varredura pré-lavratura."
---

# Varredura de vigência pré-lavratura

> Camada C1. Verificar a base; não decidir se o ato deve ser lavrado.

## Anexos obrigatórios

- `context/estado-da-norma.md`;
- `context/cnn-149-2023-compilado.md`;
- `context/uf-matriz-27.md`;
- `context/travas-defasagem.md`;
- anexo temático do ato.

## Entradas mínimas

Exigir:

- UF;
- ato/procedimento;
- modalidade presencial, eletrônica ou híbrida;
- norma/dispositivo a conferir, se indicado;
- data relevante da prática pretendida.

Sem UF, conferir somente o piso federal e impedir conclusão sobre rito estadual. Sem modalidade, marcar competência pendente.

## As quatro checagens

### A. Situação do provimento

Resolver estado, revogador, suspensão, vigência temporal e data de corte. Usar `estado-e-tipo-do-provimento`.

### B. Dispositivo no consolidado

Pesquisar o artigo no texto compilado, comparar redações empilhadas e escolher a última por data. Verificar se o caput, parágrafo ou inciso foi revogado/suspenso separadamente; o diploma pode estar vivo enquanto o dispositivo morreu.

### C. Norma da CGJ/órgão estadual

Abrir a linha da UF em `uf-matriz-27.md`. Confirmar documento-mãe, corregedoria competente, ato alterador e forma de citação. Pesquisar regra estadual que complemente, contradiga ou restrinja o piso federal.

### D. Tipo do ato normativo

Classificar como alterador, autônomo ou Resolução do Plenário. Identificar artigo-ponte e endereço correto. Não concluir que ato autônomo está ausente só porque não aparece no compilado.

## Controles especiais

1. Conferir os quatro campos de `estado-da-norma.md`: corte, último alterador, último id e suspensos.
2. Se a data atual ultrapassar o corte, rotular o resultado como **BASE DE 25/08/2026 — ATUALIDADE NÃO CONFIRMADA** até confronto oficial.
3. Vigiar remissão morta por dispositivo: MT/MS→74/2018; CE→rito revogado; RN→LC 165/1999; demais casos do anexo de travas.
4. Distinguir página de listagem, notícia, texto compilado e ato formal. Preferir o ato.
5. Não usar consolidado estadual como sinônimo de atual quando atos posteriores existirem.

## Saída do gate

Preencher:

| Campo | Resultado |
|---|---|
| UF e órgão competente | |
| ato/modalidade/data pretendida | |
| norma e dispositivo | |
| situação | vigente na base / revogado / suspenso / superado / não confirmado |
| tipo | alterador / autônomo / Resolução do Plenário |
| redação aplicável | |
| complemento estadual | |
| fonte e data de corte | |
| lacunas/conflitos | |

Finalizar com uma das fórmulas:

- **NORMA LOCALIZADA NA BASE:** apresentar o texto vigente na data de corte e devolver o juízo ao titular;
- **BLOQUEIO DE VIGÊNCIA:** norma revogada, suspensa, superada ou fonte insuficiente;
- **CHECAR ATUALIZAÇÃO:** base anterior à data de uso ou alteração posterior detectada.

## Postura obrigatória

Usar verbos **localizar, comparar, verificar, documentar e devolver**. Não usar o gate para recomendar decisão jurídica, autorizar lavratura ou produzir qualificação automática. Essa fronteira preserva a decisão final humana e atende às vedações estaduais de IA, especialmente MT.

## Reprovação automática

- vigência afirmada sem fonte/data;
- prazo/forma sem UF;
- provimento citado sem estado/tipo;
- dispositivo antigo escolhido pelo primeiro resultado;
- notícia usada para fechar vigência;
- conflito estadual omitido;
- saída “pode lavrar” em vez de relatório normativo.

## Entrega obrigatória

Entregar tabela do gate, trecho aplicável, fonte, data de corte, ressalvas e handoff ao titular. Não redigir a minuta enquanto houver bloqueio de vigência ou competência.
