---
name: calendario-de-obrigacoes-periodicas
description: "Consolida o calendário quinzenal, semestral, anual, plurianual e por evento da serventia, com RCTO, CESDI, CENSEC, eliminação, IA estadual, restauração, extração e incidentes. Esta skill deve ser usada quando o pedido mencionar agenda regulatória, prazo recorrente, obrigação periódica, correição, comunicação, treinamento, backup, restauração, pentest, extração ou incidente."
---

# Calendário de obrigações periódicas

> Camada C8. Esta skill agenda e prova cumprimento; não redige ato notarial. Base atualizada até 25/08/2026.

## Anexos e skills obrigatórios

- `context/travas-defasagem.md` — calendário consolidado e eventos;
- `context/prov-cnj-213-2026-e-anexos.md` — restauração, segurança e extração;
- `context/uf-matriz-27.md` — regime estadual;
- `comunicacao-anual-a-corregedoria`, `capacitacao-obrigatoria-em-ia`, `teste-de-extracao-integral-e-portabilidade` e `checklist-de-pre-correicao`.

## Entradas

Confirmar UF, classe da serventia, atos praticados, uso de IA, sistemas, data de vigência aplicável e último cumprimento comprovado. Não criar data-limite se o termo inicial não estiver confirmado.

## Agenda canônica

### Dias 5 e 20

- enviar RCTO e CESDI, **inclusive comunicação negativa**, conforme CNN arts. 267 e 270;
- conferir sincronização do CCN e do Índice Único da CENSEC, conforme CNN art. 311.

### Semestral

- comunicar ao juízo a eliminação de documentos, conforme Provimento CNJ 50/2015, art. 3º;
- no AM, atualizar o inventário da solução de IA;
- na Classe 3, executar e documentar teste de restauração de backup.

### Anual

- comunicar ferramentas e usos de IA à Corregedoria em MT, PI e MA, nos respectivos dispositivos estaduais;
- preparar a correição anual do CNN art. 105;
- no AM, cumprir capacitação certificada de IA de **20 horas anuais**;
- nas Classes 1 e 2, executar e documentar teste de restauração.

### A cada dois anos ou conforme a classe

- no MT, renovar a capacitação de IA a cada **24 meses**;
- na Classe 3, realizar pentest ou equivalente no mínimo a cada **dois anos**, observadas as hipóteses de relatório coletivo e dispensa condicionada;
- simular extração integral a cada **24 meses na Classe 3, 30 na Classe 2 e 36 na Classe 1**.

### Por evento

- incidente com dados pessoais: comunicar titular, ANPD, juiz corregedor permanente e CGJ em até **48 horas úteis** da ciência;
- incidente crítico de TIC: comunicar a Corregedoria em até **72 horas**;
- mudança relevante de fornecedor, arquitetura ou governança: realizar imediatamente nova simulação de extração;
- exploração ativa ou risco iminente: conter e corrigir de imediato, registrando as medidas;
- alteração normativa relevante: revisar política, contratos, riscos e calendário.

## Controle de evidência

Para cada obrigação, registrar fonte, UF, classe, período, responsável, data prevista, data cumprida, protocolo ou evidência, hash quando aplicável, pendência e próximo vencimento. Alertar antes do prazo sem presumir feriados ou regra de contagem estadual.

Não importar comunicação anual de IA para as 23 UFs que não a instituíram. Não tratar Resolução CNJ 615/2025 como obrigação própria da serventia.

## Saída

Entregar calendário filtrado, trilha de cumprimento, pendências, alertas e pacote de evidências. Separar obrigação nacional, estadual, de classe e por evento.

## Reprovação automática

- omitir negativas do RCTO ou CESDI;
- inverter periodicidade de restauração entre classes;
- chamar toda extração de bienal;
- misturar 48 horas úteis e 72 horas;
- impor comunicação estadual a outra UF;
- prometer prazo calculado sem termo inicial e contagem confirmados.
