---
name: sequencia-do-ato-esqueleto-federal
description: "Organiza o ato notarial em 14 passos, da provocação ao arquivamento, marcando cada etapa como federal, estadual ou proposta operacional e acionando os gates de UF, modalidade, competência e qualificação. Esta skill deve ser usada quando o pedido mencionar fluxo completo do ato, ordem de atendimento, passo a passo do tabelionato, protocolo, lavratura, assinatura, selo, traslado, remessas, arquivamento ou onde uma exigência entra na sequência."
---

# Sequência do ato — esqueleto federal

> Camada C3. Separar piso federal, carne estadual e organização proposta. Não apresentar rito estadual como nacional.

## Anexos e skills obrigatórios

- `context/sequencia-do-ato.md` — sequência, autoridade de cada etapa e categorias de trava;
- `context/cc-notarial.md` — validade, estrutura, representação e atos civis;
- `context/lei-8935-94.md` — atribuições, livre escolha presencial e territorialidade;
- `context/cnn-indice-de-enderecamento.md` — endereços do CNN;
- `context/travas-defasagem.md` — exceções e armadilhas;
- `roteador-uf`, `qualificacao-notarial-transversal` e `varredura-de-vigencia-pre-lavratura`.

## Legenda obrigatória

- **🇧🇷 Federal:** regra nacional efetivamente localizada;
- **🏛️ Estadual:** depende da UF e do dispositivo local;
- **⚪ Proposta:** organização operacional útil, sem pretensão normativa.

Não remover a legenda. Não converter proposta em obrigação jurídica.

## Entradas bloqueantes

Fixar UF, ato, modalidade presencial/eletrônica/híbrida, data relevante e objetivo do atendimento. Sem UF, manter somente o esqueleto federal e declarar que ele **não tem protocolo, prazo de análise, nota de exigências ou dúvida notarial**.

## Os 14 passos

1. **Provocação da parte — 🏛️/🇧🇷:** receber a rogação e delimitar o ato. O passo 1 não são custas. Não iniciar ato de ofício.
2. **Modalidade e competência — 🇧🇷:** separar presencial, eletrônico e híbrido; aplicar livre escolha e limite municipal no presencial ou competência exclusiva/absoluta no eletrônico. Declarar a lacuna do híbrido.
3. **Protocolo — 🏛️:** emitir recibo, data, hora e ordem apenas quando a UF criar protocolo notarial. Não existe protocolo federal geral.
4. **Qualificação — 🇧🇷/🏛️:** examinar identidade, capacidade, legitimidade, representação, poderes, vontade, licitude, forma, bem e titularidade; executar as consultas específicas do ato.
5. **Instrução documental — 🇧🇷:** exigir somente documentos previstos em lei e no regime estadual aplicável; usar o rol próprio do ato.
6. **Tributos — 🇧🇷/🏛️:** conferir recolhimento antes da lavratura quando a norma o exigir. Distinguir tributo de emolumento e confirmar a regra municipal do ITBI.
7. **Bifurcação — 🏛️:** qualificação positiva libera redação; negativa segue forma, prazo e destino da UF. Não existe bifurcação notarial federal com nota e dúvida.
8. **Redação e conferência da minuta — 🇧🇷/🏛️:** estruturar o instrumento pelo CC art. 215 e pela lei especial; preservar autoria e juízo do tabelião.
9. **Lavratura e leitura — 🇧🇷:** observar presença, leitura, declaração e formalidades próprias. No testamento, exigir unidade do ato e leitura específica.
10. **Assinatura e encerramento — 🇧🇷/🏛️:** colher assinaturas válidas; considerar o ato encerrado com a assinatura do tabelião e aplicar prazo estadual de ultimação quando existir.
11. **Selo — 🇧🇷/🏛️:** aplicar o regime estadual no presencial e o gate federal de nulidade do eletrônico desconforme.
12. **Traslado ou certidão — 🇧🇷:** expedir cópia fidedigna e, no eletrônico, incluir MNE e fórmula de validação.
13. **Remessas e comunicações — 🇧🇷:** cumprir CENSEC, CEP, RCTO, CESDI, UIF e comunicação ao notário emitente quando o ato exigir.
14. **Arquivamento e contas — 🇧🇷/🏛️:** guardar livros, documentos, recibos e comprovantes pelo prazo aplicável; escriturar os livros administrativos.

## Roteamento por etapa

- Acionar `primeira-etapa-e-onde-entram-as-custas` nos passos 1 e 6.
- Acionar `analise-documental-e-rol-fechado` no passo 5.
- Acionar `travas-do-ato-cinco-categorias` antes da bifurcação.
- Acionar `nota-fundamentada-de-recusa-e-encaminhamento` somente após classificar a trava.
- Acionar as skills C2 para protocolo, prazo, recusa, dúvida e emolumentos estaduais.
- Acionar a skill C4 correspondente antes da minuta.

## Saída

Entregar uma tabela com: passo, autoridade, insumo, verificação, resultado, trava e próxima skill. Marcar etapas inaplicáveis sem renumerar o fluxo. Separar pendência de documento, obstáculo externo, fato consignável e devolução institucional.

## Reprovação automática

- começar por custas ou emolumentos;
- redigir antes de modalidade e competência;
- apresentar protocolo, prazo, nota ou dúvida como federal;
- omitir a provocação da parte;
- fundir tributo e emolumento;
- ocultar o caráter proposto de uma ordem operacional;
- avançar da qualificação negativa sem classificar uma das cinco travas;
- praticar etapa registral, judicial, ministerial ou tributária em nome do tabelião.
