---
name: conformidade-de-digitalizacao
description: "Valida a digitalização do acervo pelos Anexos I e II do Decreto 10.278/2020, com resolução, formato, compressão, assinatura, metadados e cadeia de integridade. Esta skill deve ser usada quando o pedido mencionar escaneamento, PDF/A, PNG, dpi, planta, mapa, imagem, documento nato-digital, OCR, valor legal, descarte do papel ou fornecedor de digitalização."
---

# Conformidade de digitalização

## Três invioláveis

1. Nada do acervo sai sem anonimização irreversível prévia.
2. Nada alimenta treinamento: nem entrada, nem saída, nem dado inferido.
3. Nada produzido pelo plugin é ato notarial ou registral nem pode parecer ato dotado de fé pública.

Aplicar **IMUTABILIDADE, RASTREABILIDADE e RETENÇÃO MÍNIMA** em toda automação. Base normativa atualizada até 25/08/2026.

Tratar o acervo como patrimônio funcional **do serviço**, não do titular; tudo que esta skill gerar deve ser extraível em formato não proprietário, sem anuência de fornecedor. Separar a camada administrativa da camada de fé pública: nesta última, leitura autorizada pode ocorrer, mas saída com aparência de ato nunca.

## Anexos e skills obrigatórios

- `context/decreto-10278-2020.md` — requisitos e Anexos I e II;
- `context/prov-cnj-50-2015-temporalidade-notas.md` — quando a digitalização permite descarte;
- `context/prov-cnj-213-2026-e-anexos.md` — segurança, formatos abertos e continuidade;
- `plano-de-metadados` e `temporalidade-e-eliminacao`.

## Padrão técnico mínimo do Anexo I

Aplicar por tipo de original:

| Original | Resolução mínima | Formato |
|---|---:|---|
| texto impresso ou manuscrito | 300 dpi | PDF/A |
| fotografia, cartaz e imagem | 300 dpi | PNG |
| planta e mapa | 600 dpi | PNG |

Usar o modo de cor adequado ao original e compressão **sem perda**. Não converter planta ou mapa para 300 dpi. Não aceitar PDF comum como se fosse PDF/A nem extensão renomeada como validação de formato.

## Valor legal e cadeia de integridade

Para equivalência perante entidade pública, conferir cumulativamente o art. 5º do Decreto 10.278/2020: assinatura digital com certificação ICP-Brasil, padrão do Anexo I e metadados do Anexo II. Verificar também integridade e confiabilidade, rastreabilidade e auditabilidade, qualidade da imagem, confidencialidade quando cabível e interoperabilidade.

Registrar:

1. identificação do original e lote;
2. operador, equipamento, data e local;
3. parâmetros efetivos de captura;
4. validação visual e técnica;
5. hash da imagem e assinatura aplicável;
6. vínculo entre original, arquivo e metadados;
7. falhas, recapturas e aprovação;
8. exportação em formato não proprietário.

OCR serve para localizar e conferir, não para substituir a imagem nem para criar fé pública. Manter separação entre texto pesquisável e imagem probatória.

## Gate de descarte

Digitalização conforme é condição necessária quando a tabela autoriza eliminar o papel, mas não é autorização autônoma. Antes do descarte, exigir prazo cumprido, classe documental correta, regra vigente, comunicação semestral e destruição irrecuperável. **Livro de notas permanece para sempre**, mesmo digitalizado.

## Dois acervos e fornecedor

Processar a camada administrativa separada da camada de fé pública. Na segunda, limitar a automação à leitura e conferência local; a saída nunca é certidão ou traslado. Contrato e solução devem permitir extração integral, hashes, assinaturas, metadados e histórico sem anuência do fornecedor.

Não afirmar leiaute concreto de ITN não aberto. Não preencher lacuna de leiaute com padrão inventado.

## Saída

Entregar matriz de conformidade por lote, amostra validada, resolução e formato medidos, metadados, hash, assinatura, falhas, recapturas, portabilidade e decisão separada sobre elegibilidade futura de descarte. Rotular qualquer item não comprovado como pendente.

## Reprovação automática

- usar 300 dpi para plantas ou mapas;
- usar formato proprietário ou compressão com perda;
- confundir OCR com original ou ato;
- eliminar papel só porque foi escaneado;
- eliminar livro de notas;
- enviar imagem identificável a serviço externo ou treinamento;
- inventar leiaute de operador nacional.
