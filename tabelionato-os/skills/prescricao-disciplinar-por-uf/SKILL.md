---
name: prescricao-disciplinar-por-uf
description: "Roteia a prescrição disciplinar do delegatário pela UF, distinguindo 17 estados com prazo citável, 9 com ausência ou remissão insuficiente provada e RO não localizado, além de marcos e interrupções. Esta skill deve ser usada quando o pedido mencionar prescrição de PAD, decadência punitiva, data do fato, ciência da autoridade, portaria, sindicância, interrupção, prescrição intercorrente ou legislação estadual de servidores."
---

# Prescrição disciplinar por UF

> Camada C8. Errar a UF é errar a tese inteira. A Lei 8.935/1994 não fixa prazo nacional de prescrição disciplinar. Base atualizada até 25/08/2026.

## Anexos e skills obrigatórios

- `context/uf-matriz-27.md` — roteamento canônico e data de corte;
- `context/precedentes-notariais.md` — RMS 72.379/STJ;
- `context/travas-defasagem.md` — trava T-102;
- `roteador-uf`, `defesa-tecnica-em-pad` e `responsabilidade-civil-e-a-data-do-ato`.

## Gate de entrada

Exigir UF, data do fato, data em que cada autoridade tomou ciência, data e publicação da portaria, tipo de procedimento, pena máxima em tese, atos interruptivos, paralisações e decisões. Não calcular sem o texto estadual aplicável.

## Cobertura canônica 17 + 9 + 1

- **17 UFs com prazo citável:** AC, AL, AM, AP, CE, ES, GO, MA, MG, MT, PA, PI, PR, RJ, RR, RS e SP.
- **9 UFs sem prazo próprio citável ou com remissão insuficiente comprovada:** BA, DF, MS, PB, PE, RN, SC, SE e TO.
- **1 não localizada:** RO. Declarar a lacuna; não preencher por analogia automática.

Consultar os números e dispositivos em `context/uf-matriz-27.md` e na fonte estadual endereçada. A faixa vai de **seis meses no RS** a **seis anos em GO**, conforme pena e regime; não transformar extremos em regra geral.

No **PI**, aplicar a LC estadual 234/2018, art. 40: cinco anos para perda da delegação, dois anos para suspensão, um ano para multa e 180 dias para repreensão. O §1º conta da ciência pelo juiz competente ou pela Corregedoria; o §3º interrompe o prazo com a abertura de sindicância punitiva ou a instauração de PAD, até a decisão final.

## Termo inicial e interrupção

Separar os dois grupos:

- ciência ou conhecimento pela autoridade competente, oficial, formal, correcional, pelo poder público ou superior, conforme a UF;
- data do fato ou evento punível em CE, RJ e ES, além da redação vigente usada por SP.

Em **SP**, declarar a divergência interna: a lei aponta o dia da falta, mas existe orientação administrativa e literatura pela ciência. Não escolher silenciosamente. Identificar separadamente cada gatilho de interrupção; sindicância meramente preparatória pode não interromper onde a norma assim dispõe, como no PR.

## Maranhão e analogias

Preservar o caminho do MA: CODOJE e disciplina estadual, com uso argumentativo do art. 142 da Lei 8.112/1990 por analogia e referência nominada ao **PP CNJ 0006887-29.2020**. Não converter essa construção localizada em regra nacional nem omitir que a norma maranhense de 2026 passou a trazer prazos próprios.

No RS e SP, rotular expressamente a analogia com estatuto de servidores. O RMS 72.379/STJ afasta a importação automática da Lei 8.112 federal e orienta a consulta à legislação estadual.

## Dois relógios

Não misturar prescrição disciplinar com a civil. O relógio disciplinar depende da UF e pode partir da ciência ou do fato; a letra do art. 22, parágrafo único, conta o triênio civil da lavratura apenas na redação desde 2016, sujeita à *actio nata* quando a invalidação judicial materializa o dano.

## Saída

Entregar UF, autoridade, norma, pena em tese, prazo, termo inicial, interrupções, suspensões, prescrição intercorrente, cronologia e cenários. Para as nove UFs com ausência ou remissão insuficiente e, separadamente, para a lacuna de RO, emitir apenas rota de pesquisa e silêncio conclusivo.

## Reprovação automática

- afirmar prazo nacional de dois anos;
- presumir Lei 8.112/1990;
- transportar prazo ou marco entre UFs;
- esconder a divergência de SP;
- afirmar prazo próprio nas 9 ausências provadas ou em RO;
- confundir relógio disciplinar e civil;
- calcular sem pena em tese e atos interruptivos.
