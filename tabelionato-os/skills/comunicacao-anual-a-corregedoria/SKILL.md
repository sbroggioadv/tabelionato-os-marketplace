---
name: comunicacao-anual-a-corregedoria
description: "Monta a ficha anual de comunicação de uso de IA à Corregedoria conforme PI, MT ou MA, com ferramentas, finalidades, segurança, incidentes, falhas e mitigação, distinguindo a auditoria semestral do AM e a declaração federal de TIC. Esta skill deve ser usada quando o pedido mencionar relatório anual de IA, comunicar à CGJ, prestação de contas, ferramentas em uso, incidentes, mitigação, PI art. 106, MT art. 12, MA art. 170 ou auditoria semestral no Amazonas."
---

# Comunicação anual à Corregedoria

> Camada C6. Produzir ficha verificável da serventia; não inventar prazo-calendário nem confundir comunicação com auditoria.

## Anexos e skills obrigatórios

- `context/ia-por-uf.md` — regimes de reporte nas quatro UFs;
- `context/prov-cnj-213-2026-e-anexos.md` — declaração anual federal e incidentes críticos;
- `context/travas-defasagem.md` — escopo e números confirmados;
- `regime-de-ia-da-uf`, `registro-interno-de-usos-para-auditoria` e `diagnostico-de-conformidade-de-ia`.

## Gate de UF

Confirmar UF antes de gerar a ficha. Na data de corte de 25/08/2026:

- **PI, MT e MA** exigem comunicação anual estadual sobre IA;
- **AM** adota desenho distinto: auditoria semestral da própria CGJ, art. 170, I; não converter essa auditoria em relatório anual da serventia;
- nas outras **23 UFs**, não afirmar dever estadual anual de IA; aplicar apenas os reportes federais e tratar a ficha como boa prática antecipatória.

A Resolução CNJ 615/2025 não vincula a serventia por força própria. Não enviar a ficha a órgão do Judiciário previsto nessa Resolução sem norma de remissão.

## Conteúdo por UF

### Piauí — art. 106

Listar sistemas usados, propósitos e medidas adotadas para proteção de dados e segurança da informação.

### Mato Grosso — arts. 6º, V, e 12

Listar ferramentas, finalidades, incidentes registrados e medidas de mitigação. Manter coerência com o registro interno e com a comunicação de adequação quando aplicável.

### Maranhão — art. 170, §4º

Listar sistemas e finalidades, medidas de segurança, incidentes ou falhas e ações de mitigação implementadas.

Não reduzir incidente a vazamento: registrar também falha de uso ou segurança quando a norma local a alcançar.

## Conteúdo comum da ficha

1. UF, serventia por identificador institucional interno e período;
2. norma e dispositivo do reporte;
3. solução, versão, fabricante e fornecedor por categoria, sem credencial;
4. finalidade e função efetivamente usada;
5. situação `piloto | produção | suspensa | encerrada`;
6. classe de dados e arquitetura, sem reproduzir conteúdo do acervo;
7. supervisão, capacitação e revisão humana;
8. controles de segurança, auditoria, contrato e portabilidade;
9. incidentes, falhas, causa, impacto e mitigação;
10. mudanças desde o ciclo anterior, pendências e responsável pela revisão.

Usar anexos ou dossiê técnico para evidência, não despejar logs ou dados pessoais na ficha.

## Três relógios que não se confundem

- comunicação anual estadual de IA em PI, MT e MA;
- auditoria semestral conduzida pela CGJ/AM;
- declaração anual federal no Sistema Justiça Aberta, com síntese do dossiê técnico, pelo Provimento 213/2026, art. 17.

Somar as obrigações aplicáveis; uma não substitui a outra. A norma estadual lida não fixa dia ou mês uniforme para o reporte anual; não inventar 31 de dezembro ou aniversário da contratação.

## Incidente durante o ciclo

Não esperar o relatório anual para incidente que exija comunicação imediata ou em prazo próprio. Incidente crítico de TIC deve ser comunicado à Corregedoria em até **72 horas** pelo Provimento 213/2026, sem prejuízo da LGPD e das regras específicas.

## Saída

Entregar ficha anual versionada, quadro por dispositivo, relação de evidências, pendências, assinatura/revisão humana e protocolo a preencher somente após envio real. Não simular recibo nem afirmar que a Corregedoria recebeu.

## Reprovação automática

- exigir relatório anual estadual no AM ou nas outras 23 UFs;
- omitir incidentes e mitigação no MT ou MA;
- confundir auditoria semestral com comunicação anual;
- aguardar o ciclo anual para incidente crítico;
- inventar data uniforme de entrega;
- despejar log, prompt ou PII no relatório;
- afirmar protocolo sem comprovante;
- aplicar a Resolução 615 diretamente.
