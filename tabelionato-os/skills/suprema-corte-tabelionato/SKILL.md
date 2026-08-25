---
name: suprema-corte-tabelionato
description: "Gate adversarial default-on do tabelionato-os. Audita a saída do plugin em quatro rodadas: R1 vigência e classificação do ato normativo, R2 destinatário correto, R3 separação federal e estadual com UF, e R4 postura de verificar, documentar e devolver sem decidir. Esta skill deve ser usada antes de entregar minuta, checklist, orientação ou relatório, ou quando o pedido mencionar revisão final, conferir fundamento, norma vigente, destinatário, pode entregar, auditar R1-R4, suprema corte ou /suprema-corte-tabelionato."
---

# Suprema Corte Tabelionato — gate R1-R4

> Camada C0. Auditar a **saída do plugin**, nunca aprovar o ato nem substituir o juízo do titular. Rodar por padrão antes de qualquer entrega.

## Anexos obrigatórios

- `context/estado-da-norma.md`;
- `context/cnn-149-2023-compilado.md`;
- `context/cnn-indice-de-enderecamento.md`;
- `context/uf-matriz-27.md`;
- `context/travas-defasagem.md`;
- anexo temático citado na saída.

Localizar e ler a faixa de cada fundamento auditado.

## Objetivo

Devolver um veredito sobre a qualidade da resposta:

- **SAÍDA LIBERADA:** R1, R2, R3 e R4 sem falha;
- **CORRIGIR SAÍDA:** pelo menos uma falha, com trecho reprovado, razão e substituto ancorado.

“Saída liberada” não significa autorização para lavrar; significa apenas que o texto do plugin passou pelos quatro controles.

## R1 — Vigência

Para cada ato normativo citado:

1. Registrar a data de corte do contexto.
2. Resolver o **estado**: absorvido/revogado, vivo por remissão ou suspenso.
3. Resolver o **tipo**: alterador, autônomo ou Resolução do Plenário.
4. Conferir a redação mais recente do dispositivo no consolidado.
5. Conferir remissão a ato anterior e eventual norma superveniente.
6. Reconciliar citações do mesmo fato entre onboarding, diagnóstico e skill operacional; divergência de artigo para a mesma régua bloqueia a saída até confronto com o anexo verbatim.

Reprovar automaticamente:

- afirmação de vigência sem data de corte;
- “suspenso” tratado como “revogado” ou plenamente vigente;
- Resolução do Plenário apresentada como parte do CNN;
- Provimento 74/2018 usado como norma viva em cláusula de MT/MS;
- Provimento 244/2026 chamado de alterador do CNN;
- número de alterações diferente de 57 na fotografia de 25/08/2026;
- trecho antigo escolhido apenas por aparecer empilhado no compilado.
- régua de classes do Provimento CNJ 213/2026 citada fora do art. 16 ou com endereços divergentes entre skills.

Na data de corte, registrar como suspensos ativos os Provimentos 172/2024, 175/2024 e 247/2026; tratar a data aproximada de 12/10/2026 do último como alerta de nova checagem, não como certeza permanente.

## R2 — Destinatário

Perguntar para cada norma: **quem recebe o comando?** Delegatário de Notas, registrador, tabelião de Protesto, magistrado, servidor, unidade do tribunal ou fornecedor?

Reprovar:

- uso interno de IA do tribunal apresentado como norma para serventia;
- ES Prov. 21/2019, BA Decreto 1007/2025, CE Portaria 03/2026, PI Prov. 151/2023 ou AM Resolução 29/2026 usados como regime de IA do delegatário;
- SC art. 112 da LC 339/2006 usado como prescrição do delegatário, pois alcança magistrado;
- PR art. 765 usado para Notas, pois está no Protesto;
- CE art. 172 estendido ao notário sem ressalva, pois nomina o registrador;
- Resolução CNJ 615/2025 aplicada diretamente à serventia sem ponte normativa estadual;
- fase do Registro de Imóveis, do MP ou do juízo executada como se fosse notarial.

## R3 — UF e camada normativa

1. Confirmar UF no pedido ou no perfil.
2. Separar piso federal, norma estadual e eventual regra municipal.
3. Conferir documento-mãe e corregedoria competente em `uf-matriz-27.md`.
4. Conferir forma de citação e contagem de prazo da UF.
5. Marcar lacunas e selos 🟡/🔴 sem preenchê-los.

Reprovar:

- prazo, protocolo, recusa, dúvida, IA ou emolumento estadual sem UF;
- norma estadual apresentada como nacional;
- regra federal omitida por existir regra estadual;
- prazo em dias úteis/corridos transportado entre UFs;
- “Código da CGJ” presumido em PI, MA, BA, GO, SC, PA, RO ou TO;
- categoria A3 apresentada como rito geral ou categoria B/C apresentada como dúvida notarial ampla;
- valor de emolumento em reais.

## R4 — Postura

Auditar verbos e limites. Preferir:

- **verificar** situação, competência, documento e condição;
- **documentar** fonte, data, ressalva, recusa e consulta;
- **devolver/remeter** controvérsia ao titular ou órgão competente.

Reprovar saídas que:

- decidam a qualificação no lugar do titular;
- recomendem ou sugiram decisão jurídica produzida por IA;
- prometam aprovação, homologação, registro, correição ou resultado;
- inventem rito para arbitragem, precatório, ato híbrido ou lacuna estadual;
- tratem checklist/minuta preliminar como ato ou decisão final;
- omitam que a competência humana é indelegável.

## Metodologia

1. Rodar R1 → R2 → R3 → R4 nessa ordem.
2. Marcar cada item **OK** ou **CORRIGIR**.
3. Citar arquivo e fundamento da correção.
4. Devolver à skill de origem quando houver falha; não entregar o artefato reprovado.
5. Liberar somente com as quatro rodadas em OK.

## Entrega obrigatória

Emitir:

1. veredito;
2. tabela R1-R4 com evidência concisa;
3. correções bloqueantes e texto substituto;
4. pendências que exigem atualização ou decisão humana.

## Guard

Não “passar pano”. Ausência de prova não vira aprovação. Item posterior à data de corte permanece **CHECAR VIGÊNCIA** até confronto com fonte oficial; saída assim marcada não pode afirmar atualidade.
