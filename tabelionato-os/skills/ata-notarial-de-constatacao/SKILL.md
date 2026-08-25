---
name: ata-notarial-de-constatacao
description: "Conduz ata notarial de constatação com base no CPC art. 384 e na exclusividade da Lei 8.935/1994, delimitando fatos percebidos pessoalmente, competência, diligência, cadeia de evidência e três cláusulas propostas sem criar eficácia jurídica. Esta skill deve ser usada quando o pedido mencionar ata notarial, constatação de fato, prova digital, conteúdo de site ou mensagem, diligência, e-Not Provas, alerta de falsidade, cláusula de não-eficácia ou descrição imparcial pelo tabelião."
---

# Ata notarial de constatação

> Camada C4. Autenticar fatos constatados; não concluir direitos, ilícitos, autoria ou eficácia.

## Anexos e skills obrigatórios

- `context/lei-8935-94.md` — competência exclusiva para atas;
- `context/cc-notarial.md` — força probante e limites civis;
- `context/travas-defasagem.md` — travas T-47 a T-52;
- `context/cnn-indice-de-enderecamento.md` — atas especiais e fronteiras;
- `sequencia-do-ato-esqueleto-federal` e `ato-notarial-eletronico-e-competencia`.

## Limite normativo

Usar CPC art. 384 e Lei 8.935/1994, art. 7º, III, como âncoras nacionais. Declarar que não existe capítulo nacional geral da ata de constatação; forma adicional, diligência e conteúdo dependem da UF.

Não apresentar como norma nacional um modelo extraído de usucapião ou adjudicação.

## Entradas

Fixar UF, modalidade, fato a constatar, local físico/digital, data e horário, acesso lícito, origem do material, pessoas presentes e finalidade declarada. Excluir pedido de investigação, perícia, inferência de autoria ou opinião jurídica.

## Competência e objeto

No presencial, observar limite municipal da diligência. No eletrônico, aplicar competência exclusiva da circunscrição do fato constatado ou, inaplicável, do domicílio do requerente. Não transportar livre escolha presencial.

Delimitar o objeto em verbos perceptivos: acessar, visualizar, ouvir, navegar, receber, comparar, registrar. Descrever somente o que o tabelião percebeu e os passos reproduzíveis.

## Protocolo de constatação

1. Registrar rogação, escopo e finalidade declarada.
2. Confirmar competência, acesso e licitude da diligência.
3. Identificar ambiente, dispositivo, conexão, data e horário relevantes sem coletar dado excessivo.
4. Descrever a sequência de ações e o conteúdo observado em ordem cronológica.
5. Preservar arquivos, capturas e metadados permitidos com rastreabilidade.
6. Distinguir declaração do requerente de percepção direta do tabelião.
7. Inserir limites técnicos, inacessibilidades e mudanças durante a diligência.
8. Ler, assinar, selar, expedir e arquivar conforme modalidade e UF.

## Três cláusulas propostas

Inserir, quando adequadas, marcadas como **⚪ PROPOSTA OPERACIONAL**:

- alerta ao requerente e testemunhas sobre responsabilidade por falsidade;
- ressalva de que a ata não cria eficácia jurídica, propriedade ou validade do conteúdo;
- ressalva de que a conclusão não se baseia apenas na declaração do requerente.

Essas cláusulas derivam de modelos nacionais específicos dos arts. 402 e 440-G; não atribuir-lhes força de norma geral. Não usar a cláusula de não-eficácia na ata de arrematação hipotecária, que possui função translativa própria.

## Fronteiras entre atas

- **Usucapião:** competência vinculada e vedação de base exclusiva na declaração; acionar skill própria.
- **Adjudicação:** regras e ressalvas diferentes; acionar skill própria.
- **Arrematação hipotecária:** título translativo; não copiar cláusulas das anteriores.
- **Conta notarial:** documentar divergência sem decidir eficácia ou rescisão.

## e-Not Provas

Não tratar e-Not Provas como sinônimo de ata. A captura self-service do cliente não contém diligência pessoal do tabelião; a ata do art. 384 documenta a constatação notarial e sua responsabilidade própria.

## Saída

Entregar roteiro de diligência, matriz fato percebido/fonte/horário, limites, lista de anexos e estrutura de ata. Não preencher conteúdo que não tenha sido efetivamente observado.

## Reprovação automática

- concluir crime, autoria, direito ou eficácia;
- usar declaração do requerente como constatação exclusiva;
- apresentar norma estadual ou cláusula proposta como nacional;
- confundir e-Not Provas com ata;
- ignorar competência territorial;
- transportar cláusula de usucapião/adjudicação/arrematação;
- coletar dado sem necessidade;
- redigir fato não observado.
