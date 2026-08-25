---
name: usucapiao-extrajudicial-fase-notarial
description: "Conduz exclusivamente a fase notarial da usucapião extrajudicial, delimitando competência territorial, conteúdo probatório, advertência de falsidade, ressalva de não propriedade e fronteira com o processo do Registro de Imóveis. Esta skill deve ser usada quando o pedido mencionar ata de usucapião, tempo ou cadeia de posse, testemunha, diligência no imóvel, art. 216-A da LRP, CNN arts. 401 a 423, Reurb-S, notificação de confrontante ou processo registral de usucapião."
---

# Usucapião extrajudicial — fase notarial

> Camada C5. O tabelião de notas produz a ata instrutória; não processa nem decide a usucapião.

## Anexos e skills obrigatórios

- `context/cnn-149-2023-compilado.md` — CNN arts. 401 a 423;
- `context/travas-defasagem.md` — competência, prova, RO e atos autônomos;
- `context/uf-matriz-27.md` — regra procedimental estadual, inclusive RO;
- `context/sequencia-do-ato.md` — fluxo notarial;
- `roteador-uf`, `ata-notarial-de-constatacao`, `qualificacao-notarial-transversal` e `emolumentos-norma-da-uf`.

## Entradas bloqueantes

Fixar UF, município e localização da maior parte do imóvel, matrícula ou descrição da área, requerente e cônjuge ou companheiro, titular tabular, cadeia e modalidade de posse, antecessores, modalidade de usucapião e base legal, documentos, testemunhas, valor e necessidade de diligência. Não escolher modalidade jurídica por lacuna factual.

## Competência vinculada

Aplicar CNN art. 402: lavrar pelo tabelião de notas do município onde estiver o imóvel ou a maior parte dele. Não aplicar a livre escolha da adjudicação compulsória nem a fórmula da circunscrição delegada da arrematação hipotecária. Atas complementares e escrituras declaratórias podem vir de notários diversos nas hipóteses do art. 401, §7º, mas isso não altera a competência da ata principal.

## Conteúdo e prova

Conferir no mínimo:

- qualificação, domicílio e endereço eletrônico do requerente, cônjuge ou companheiro e titular tabular;
- descrição do imóvel ou da área, com edificações, benfeitorias e acessões;
- tempo, características e cadeia da posse do requerente e antecessores;
- forma de aquisição da posse;
- modalidade pretendida e base legal ou constitucional;
- número de imóveis e circunscrições atingidas;
- valor do imóvel;
- demais elementos necessários, inclusive depoimentos.

Não basear a ata apenas em declarações do requerente. Incorporar documentos, imagens, sons, testemunhas, confrontantes e diligência quando necessários. Alertar requerente **e testemunhas** de que declaração falsa configura crime de falsidade.

## Ressalva obrigatória

Consignar que a ata **não confirma nem estabelece propriedade** e serve somente para instruir o requerimento extrajudicial perante o Registro de Imóveis. Não aproveitar a cláusula translativa da arrematação hipotecária.

## Fase notarial × fase registral

### Tabelião de notas

Qualificar, colher e confrontar provas, fazer diligência facultativa, lavrar a ata, advertir sobre falsidade e inserir a ressalva de não propriedade.

### Oficial do Registro de Imóveis

Autuar e prenotar, notificar titulares e confrontantes, publicar edital, cientificar entes públicos, tratar impugnação, promover conciliação ou mediação, decidir, suscitar dúvida quando provocado, registrar e abrir matrícula. Não praticar no tabelionato nenhuma dessas etapas registrais.

## Regra estadual sem transporte

Acionar `roteador-uf` antes de informar protocolo ou prazo. Em RO, tratar como regras registrais locais: análise do art. 836 em 10 dias úteis, diligência do art. 837 em 10 dias úteis e ato do art. 838 em 10 dias úteis, preservada a exceção expressa da Reurb-S. Não transformar esses prazos em regra nacional nem em prazo do tabelião.

## Emolumentos

Tratar diligências, reconhecimentos, escrituras declaratórias, notificações e demais atos preparatórios ou instrutórios como atos autônomos conforme CNN art. 423, parágrafo único, com despesas adiantadas pelo requerente e valores definidos pela legislação local. Não informar número memorizado.

## Saída

Entregar decisão de competência, matriz de conteúdo e prova, advertências, diligências, ressalva obrigatória, custos por categoria sem valores e quadro explícito “fase notarial / fase registral”.

## Reprovação automática

- processar usucapião no tabelionato;
- aplicar livre escolha ao ato principal;
- basear a ata apenas na declaração do requerente;
- omitir advertência ao requerente ou às testemunhas;
- dizer que a ata transfere ou confirma propriedade;
- atribuir notificação, edital, decisão ou registro ao tabelião;
- transportar prazos de RO a outra UF.
