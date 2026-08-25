---
name: clausula-de-meios-e-formas-de-pagamento
description: "Estrutura a cláusula obrigatória do CNN art. 165-A para direitos reais imobiliários, detalhando cinco meios de pagamento, terceiro pagador, parcelas, condição de PEP e consignação da recusa em informar, com a remissão 155/155-A declarada. Esta skill deve ser usada quando o pedido mencionar forma de pagamento na escritura, transferência, cheque, espécie, ativo virtual, dação, permuta, terceiro pagador, pagamento parcelado, recusa em informar, PEP, PLD ou comunicação à UIF."
---

# Cláusula de meios e formas de pagamento

> Camada C4. Aplicar o CNN art. 165-A em toda escritura de constituição, alienação ou oneração de direito real sobre imóvel.

## Anexos e skills obrigatórios

- `context/cnn-149-2023-compilado.md` — versão e vigência do Código;
- `context/cnn-indice-de-enderecamento.md` — endereço PLD/Notas;
- `context/travas-defasagem.md` — travas T-32, T-41 e T-42;
- `context/estado-da-norma.md` — gate temporal;
- `travas-do-ato-cinco-categorias` e `escritura-publica`.

## Entradas

Fixar negócio, imóvel, preço documentado, todos os meios usados, datas/locais, parcelas, contas ou títulos envolvidos, titulares, terceiro pagador, condição de PEP e eventual recusa em fornecer informação. Processar somente categorias e fatos entregues; não expor dados pessoais na resposta-modelo.

## Cinco incisos do §1º

Organizar:

1. **Espécie:** mencionar expressamente local, data e valor documentado.
2. **Transferência bancária:** identificar inequivocamente contas de origem/destino, titulares, datas e valores.
3. **Cheque:** registrar elementos de identificação, conta de origem e eventual destino, titulares, data e valores.
4. **Outros meios:** identificar cotas/ações, cessões, títulos, ativos virtuais, dação, permuta, prestação de serviço ou outro meio, com local, data, origem e destino.
5. **Parcelamento:** discriminar o meio de cada parcela com os dados do inciso correspondente.

Não resumir como “pago e quitado”. Não omitir parcela ou combinar meios heterogêneos sem discriminação.

## Terceiro pagador

Quando contas ou recursos pertencerem a terceiro, qualificar o terceiro na escritura conforme §2º e documentar a relação declarada com o negócio. Não inferir beneficiário, titularidade ou origem de recursos.

## Recusa em informar — categoria D

Aplicar o §3º: mencionar a recusa na escritura. Não recusar a lavratura apenas pela falta de informação obtida exclusivamente em razão do capítulo de PLD. Constituir prova da resistência e comunicar à UIF quando o enquadramento aplicável assim exigir.

Tratar a hipótese como **CONSIGNÁVEL**: lavrar, consignar e comunicar. Não converter em exigência sanável ou declaração inventada.

## Duas tensões do CNN

### Remissão 155 × 155-A

Citar literalmente que o §3º remete ao art. 155, VIII e declarar que o art. 155 foi revogado pelo mesmo Provimento 161/2024. Apontar que o conteúdo vivo sobre resistência ao fornecimento está no art. 155-A, VIII. Não corrigir silenciosamente a remissão nem repetir artigo revogado como vigente.

### Art. 109 × art. 165-A

Não citar o art. 109 isoladamente para dispensar condição de PEP. Declarar a tensão com o art. 165-A, posterior e específico para escrituras de direitos reais imobiliários, sem esconder a divergência.

## Modelo de saída

Produzir quadro seguro antes da cláusula:

| Parcela/meio | Categoria | Data/local | Origem | Destino | Titular/terceiro | Prova | Pendência |
|---|---|---|---|---|---|---|---|

Depois, redigir uma cláusula individualizada que:

- cubra os cinco incisos aplicáveis;
- qualifique terceiro pagador;
- registre PEP conforme a regra específica;
- consigne eventual recusa sem criar fato;
- indique comunicação separada, sem narrar análise sigilosa no instrumento além do necessário.

## Reprovação automática

- omitir meio ou parcela;
- usar cláusula genérica de quitação;
- inventar origem, conta, terceiro ou condição PEP;
- recusar ato apenas pela resistência informacional;
- transformar consignável em sanável;
- citar o art. 155 como vigente sem ressalva;
- substituir silenciosamente 155 por 155-A;
- citar o art. 109 sozinho;
- expor análise de UIF ou dado sigiloso além do necessário.
