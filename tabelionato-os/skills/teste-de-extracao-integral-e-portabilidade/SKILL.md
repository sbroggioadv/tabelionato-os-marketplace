---
name: teste-de-extracao-integral-e-portabilidade
description: "Planeja e documenta a extração integral, autônoma e migrável do acervo em formato interoperável e não proprietário, sem anuência do fornecedor, para provar continuidade e transferência ao sucessor. Esta skill deve ser usada quando o pedido mencionar migração, troca de sistema, portabilidade, reversibilidade, exportação, sucessão, vendor lock-in, homologação, teste de extração ou reconstrução do acervo."
---

# Teste de extração integral e portabilidade

## Três invioláveis

1. Nada do acervo sai sem anonimização irreversível prévia.
2. Nada alimenta treinamento: nem entrada, nem saída, nem dado inferido.
3. Nada produzido pelo plugin é ato notarial ou registral nem pode parecer ato dotado de fé pública.

Aplicar **IMUTABILIDADE, RASTREABILIDADE e RETENÇÃO MÍNIMA** em toda automação. Base normativa atualizada até 25/08/2026.

Tratar o acervo como patrimônio funcional **do serviço**, não do titular; tudo que esta skill gerar deve ser extraível em formato não proprietário, sem anuência de fornecedor. Separar a camada administrativa da camada de fé pública: nesta última, leitura autorizada pode ocorrer, mas saída com aparência de ato nunca.

## Anexos e skills obrigatórios

- `context/prov-cnj-213-2026-e-anexos.md` — autonomia, portabilidade e Anexo IV;
- `context/decreto-10278-2020.md` — interoperabilidade, imagem e metadados;
- `plano-de-metadados`, `classificacao-por-classe-e-plano-de-tic` e `diagnostico-do-acervo`.

## Resultado jurídico-técnico

Provar a **extração integral, autônoma e documentada** do acervo em formato interoperável, sem necessidade de anuência ou intervenção do fornecedor. A prova deve permitir reconstrução e transferência organizada ao sucessor, conforme Provimento CNJ 213/2026, art. 6º, III.

O acervo é do serviço. Contrato, criptografia, chave, licença ou API não podem transformar o fornecedor, o titular atual ou o plugin em porteiro da continuidade.

## Quando testar

- Classe 3: no mínimo a cada **24 meses**;
- Classe 2: no mínimo a cada **30 meses**;
- Classe 1: no mínimo a cada **36 meses**;
- todas as classes: **imediatamente** após alteração relevante de fornecedor, arquitetura tecnológica ou modelo de governança.

Não chamar todas as classes de bienais. A não demonstração de viabilidade impede a homologação da etapa de conformidade.

## Plano do teste

1. Delimitar sistemas, bancos, documentos, imagens, metadados, índices, logs, configurações, acessos e histórico.
2. Congelar o ponto de corte e registrar volumes, versões, esquemas e hashes de referência.
3. Executar a exportação sem assistência ou consentimento do fornecedor.
4. Validar formatos abertos, completude, relacionamentos, identificadores, assinaturas e hashes.
5. Reconstruir em ambiente isolado ou de contingência e realizar buscas representativas.
6. Comparar contagens, amostras, cadeia de integridade, permissões e trilhas antes/depois.
7. Medir tempo, dependências, falhas, itens não exportados e capacidade de continuidade.
8. Assinar relatório, plano de correção e evidências com responsável técnico.

Admitir execução segmentada por módulo ou base apenas quando evidência técnica formal demonstrar reconstrução integral. Amostragem valida consistência; não converte exportação parcial em integral.

## Dois acervos e ambiente

Separar dados administrativos dos dados de fé pública e preservar controles de acesso. Em teste fora do ambiente produtivo, usar cópia protegida; qualquer saída externa precisa estar irreversivelmente anonimizada. Dados de fé pública não podem ser usados para treinamento, avaliação de modelo ou demonstração comercial.

## Checklist contratual

Exigir reversibilidade integral, formato estruturado e não proprietário, documentação técnica, preservação de chaves e hashes, cooperação na transição, gestão de incidentes e exclusão segura de cópias do fornecedor depois da migração. Cooperação pode existir; **anuência como condição não pode**.

## Saída

Entregar escopo, ponto de corte, procedimento, evidências, reconciliação quantitativa e qualitativa, tempo de reconstrução, falhas, correções, atestado de independência e decisão de homologação. Classificar “integral”, “parcial” ou “não demonstrado” sem maquiagem.

## Reprovação automática

- exigir anuência ou intervenção do fornecedor;
- exportar só PDF e omitir metadados, vínculos ou histórico;
- declarar integralidade por amostra;
- aplicar ciclo de 24 meses a todas as classes;
- transportar dado identificável a ambiente externo;
- homologar sem evidência de transferência ao sucessor.
