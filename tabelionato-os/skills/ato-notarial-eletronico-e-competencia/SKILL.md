---
name: ato-notarial-eletronico-e-competencia
description: "Aplica os cinco requisitos do ato eletrônico, roteiro obrigatório da videoconferência, algoritmo de competência absoluta, nulidades por assinatura fora do e-Notariado ou selo ausente e MNE de 24 dígitos, declarando a lacuna do híbrido. Esta skill deve ser usada quando o pedido mencionar e-Notariado, escritura ou procuração eletrônica, ata remota, videoconferência, competência territorial eletrônica, domicílio, circunscrição, assinatura remota, selo, MNE, certificado notarizado ou ato híbrido."
---

# Ato notarial eletrônico e competência

> Camada C4. Tratar competência, e-Notariado e selo como gates anteriores à minuta. Livre escolha presencial não governa o eletrônico.

## Anexos e skills obrigatórios

- `context/cnn-indice-de-enderecamento.md` — núcleo eletrônico nos arts. 264-319;
- `context/cnn-149-2023-compilado.md` — versão do CNN;
- `context/estado-da-norma.md` — vigência e suspensões;
- `context/travas-defasagem.md` — travas T-28 e T-66 a T-70;
- `roteador-uf`, `varredura-de-vigencia-pre-lavratura` e a skill material do ato.

## Entradas bloqueantes

Fixar UF, tipo de ato, modalidade eletrônica ou híbrida, localização do imóvel/fato, domicílio comprovado das partes relevantes, circunscrições, identidade, certificado, plataforma, selo estadual e dados para MNE. Não redigir antes de resolver competência.

## Cinco requisitos do CNN art. 286

Exigir cumulativamente:

1. videoconferência notarial para captar consentimento;
2. concordância expressa das partes com o ato;
3. assinatura digital das partes exclusivamente pelo e-Notariado;
4. assinatura do tabelião com certificado ICP-Brasil;
5. formato documental de longa duração com assinatura digital.

Todos os tabeliães de notas devem prestar o serviço eletrônico conforme art. 284, parágrafo único. Não converter obrigatoriedade do serviço em liberdade para atuar fora da competência.

## Roteiro obrigatório da videoconferência

Gravar e declarar os cinco itens mínimos:

1. identificação, capacidade e livre manifestação atestadas pelo tabelião;
2. consentimento e concordância com o instrumento;
3. objeto e preço do negócio;
4. data e horário;
5. livro, página e tabelionato da lavratura.

Não substituir fala/gravação por checkbox interno.

## Algoritmo de competência

### Escritura eletrônica

1. Identificar circunscrição do imóvel e domicílio comprovado do adquirente.
2. Havendo imóveis em circunscrições diferentes no mesmo ato, admitir tabelião de qualquer delas.
3. Estando imóvel e domicílio do adquirente na mesma UF, admitir escolha de qualquer tabelionato dessa UF.
4. Sem prova do domicílio da pessoa física, usar apenas o local do imóvel.

Aplicar a ordem do art. 302, §3º, para definir adquirente. Para pessoa jurídica, comprovar sede da matriz ou filial ligada ao negócio.

### Ata e procuração eletrônicas

- Ata: circunscrição do fato constatado; se inaplicável, domicílio do requerente.
- Procuração: domicílio do outorgante ou local do imóvel, quando for o caso.

Tratar a competência como exclusiva e absoluta, conforme arts. 289 e 302-304. Não aplicar o art. 8º da Lei 8.935/1994.

## Duas nulidades expressas

- Bloquear assinatura eletrônica a distância fora do e-Notariado, conforme art. 318.
- Considerar nulo o ato eletrônico sem selo exigido pela norma estadual/distrital, conforme art. 319, §1º.

Não aceitar plataforma privada ou conta gov.br como substituto do e-Notariado para assinatura do ato.

## MNE e validação

Gerar MNE com 24 dígitos em seis campos e dois verificadores pelo Módulo 97 Base 10, ISO 7064:2003. Fazer o número integrar o ato e todas as cópias. Incluir nos traslados/certidões a expressão obrigatória de consulta de validade.

Não inventar MNE sem os dados da serventia e do ato. Validar o cálculo antes da expedição.

## Ato híbrido

Reconhecer que o art. 313 autoriza uma assinatura física e outra a distância. Declarar que o texto não resolve se a competência segue os arts. 302-304 ou a livre escolha presencial. Não escolher uma das leituras; solicitar orientação correcional ou jurídica específica.

## Saída

| Gate | Resultado |
|---|---|
| tipo/modalidade | |
| competência e prova | |
| cinco requisitos | |
| cinco itens da gravação | |
| assinatura e plataforma | |
| selo estadual | |
| MNE/validação | |
| híbrido/lacuna | |

## Reprovação automática

- usar livre escolha presencial no eletrônico;
- minutar antes da competência;
- omitir requisito ou item da videoconferência;
- aceitar assinatura remota fora do e-Notariado;
- lavrar sem selo exigido;
- informar MNE com quantidade/algoritmo errados;
- resolver o híbrido por analogia;
- expandir dispensa de selo para módulos não listados.
