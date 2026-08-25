---
name: prazos-e-protocolo-por-uf
description: "Monta o relógio estadual do ato notarial com número, marco inicial, unidade, evento de parada e consequência, preservando o ciclo completo do PI, os prazos de MG/PB, a janela do RJ e contagens úteis ou corridas por UF. Esta skill deve ser usada quando o pedido mencionar protocolo, prazo de análise, nota de exigências, prazo para assinatura, reanálise, dúvida, dias úteis, dias corridos, termo inicial, data-limite ou ato incompleto."
---

# Prazos e protocolo por UF

> Camada C2. Um prazo só existe com UF, evento, número, unidade e dispositivo. Não existe relógio federal geral de análise notarial.

## Anexos obrigatórios

- `context/uf-matriz-27.md` — categoria, endereço e regra de contagem;
- `context/sequencia-do-ato.md` — evento inicial e posição do relógio;
- `context/travas-defasagem.md` — alterações recentes, assimetrias e falsos positivos;
- `context/estado-da-norma.md` — vigência da redação usada.

## Entradas bloqueantes

Exigir:

1. UF;
2. ato ou procedimento;
3. evento que pode iniciar o prazo — protocolo, apresentação, ciência, assinatura ou outro;
4. data comprovada do evento, se houver cálculo;
5. eventual nota, reapresentação, requerimento de dúvida ou documento novo;
6. feriados e suspensão local quando a contagem for necessária.

Sem UF, responder somente: **“O esqueleto federal não tem protocolo, prazo nem nota de exigências para o tabelionato de notas.”** Não calcular data-limite.

## Algoritmo

### 1. Identificar o tipo de relógio

Separar prazo de análise, emissão da nota, atendimento pelo interessado, reanálise, assinatura, suscitação, manifestação no rito e guarda. Não somar prazos de objetos diferentes nem usar prazo disciplinar, registral ou judicial como prazo notarial.

### 2. Fixar os quatro eixos locais

Para cada relógio, registrar:

- número;
- marco inicial;
- dias úteis ou corridos;
- consequência do decurso.

Declarar “não fixado” quando a norma remeter sem número. Declarar “não localizado” quando a cobertura não permitir conclusão. Não substituir nenhuma das duas situações por prazo razoável.

### 3. Aplicar os prazos notariais comprovados

Preservar os seis prazos com número fixado no ciclo A1:

- PI: 10 dias úteis do protocolo;
- PA: 15 dias da apresentação, em dias corridos;
- TO: 15 dias da apresentação, em dias corridos;
- CE: 10 dias úteis, no marco definido pelo art. 163;
- MG: 10 dias do protocolo, em dias corridos, na redação posterior ao Provimento Conjunto 142/2025;
- PB: 10 dias úteis do protocolo, na redação posterior ao Provimento 100/2025.

Não acrescentar RR ao grupo: “prazo legal” não fixa número. Não acrescentar MA: “prazos normativos respectivos” é remissão sem número. No AP, registrar que o art. 231 prevê 10 dias úteis para “o oficial”, enquanto os dispositivos seguintes alcançam notário e oficial; não afirmar o prazo ao tabelião sem ressalva.

### 4. Executar o ciclo completo do PI

Aplicar, quando o caso for PI:

1. análise em 10 dias úteis do protocolo;
2. disponibilização para assinatura ou nota escrita;
3. assinatura em até 20 dias úteis, sob pena de ato incompleto;
4. após a nota, 10 dias úteis para o interessado apresentar documentos ou requerer suscitação;
5. reapresentados os documentos, nova análise em 5 dias úteis.

Não projetar esse ciclo para outra UF. O PI é a única UF com os dois lados do relógio fechados no corpus.

### 5. Aplicar relógios especiais

- **RJ:** preservar os 5 dias do interessado para requerer remessa da recusa ao juízo; sem requerimento, declarar o ato incompleto e sem emolumentos. Separar esse prazo do prazo de análise, que não foi fixado.
- **Assinatura:** PI usa 20 dias úteis; DF e RJ usam 30 dias para ultimarem o ato, com a consequência local de certificação/incompletude.
- **Contagem geral:** PR e MS usam dias úteis nos endereços indicados; SC, MT e SE possuem regras de dias corridos/contínuos nos respectivos procedimentos. Conferir o escopo antes de aplicar.
- **RO:** os prazos localizados são específicos da usucapião; não convertê-los em prazo geral da recusa notarial.

### 6. Calcular somente com calendário suficiente

Confirmar data, horário de protocolo quando relevante, feriados e regra de inclusão/exclusão. Se faltar qualquer insumo, entregar a fórmula do relógio sem produzir data final. Citar norma e redação temporal antes do resultado.

## Saída

| Relógio | Número | Marco | Unidade | Interrupção/suspensão | Consequência | Fonte |
|---|---:|---|---|---|---|---|
| análise | | | | | | |
| interessado | | | | | | |
| reanálise | | | | | | |
| assinatura | | | | | | |
| dúvida | | | | | | |

Encerrar com as lacunas e a redação vigente utilizada.

## Reprovação automática

- afirmar prazo sem UF;
- omitir marco ou unidade;
- usar versão antiga de MG ou PB;
- transformar remissão de RR ou MA em número;
- omitir a assimetria do AP;
- confundir os cinco dias do RJ com análise;
- transportar o ciclo completo do PI;
- calcular data sem calendário suficiente;
- tratar dias úteis e corridos como equivalentes.
