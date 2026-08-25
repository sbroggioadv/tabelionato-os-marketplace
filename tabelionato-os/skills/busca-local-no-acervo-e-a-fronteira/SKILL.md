---
name: busca-local-no-acervo-e-a-fronteira
description: "Desenha busca e sumarização locais no acervo sob a autorização tecnológica do Provimento CNJ 213/2026, impondo imutabilidade, rastreabilidade, retenção mínima e a fronteira entre localizar e praticar ato. Esta skill deve ser usada quando o pedido mencionar IA sobre acervo, busca semântica, RAG, embeddings, indexação local, sumarização, pesquisa documental, agente, modelo ou consulta ao acervo."
---

# Busca local no acervo e a fronteira

## Três invioláveis

1. Nada do acervo sai sem anonimização irreversível prévia.
2. Nada alimenta treinamento: nem entrada, nem saída, nem dado inferido.
3. Nada produzido pelo plugin é ato notarial ou registral nem pode parecer ato dotado de fé pública.

Aplicar **IMUTABILIDADE, RASTREABILIDADE e RETENÇÃO MÍNIMA** em toda automação. Base normativa atualizada até 25/08/2026.

Tratar o acervo como patrimônio funcional **do serviço**, não do titular; tudo que esta skill gerar deve ser extraível em formato não proprietário, sem anuência de fornecedor. Separar a camada administrativa da camada de fé pública: nesta última, leitura autorizada pode ocorrer, mas saída com aparência de ato nunca.

## Anexos e skills obrigatórios

- `context/prov-cnj-213-2026-e-anexos.md` — Anexo II, item 3, VI;
- `context/res-cnj-615-2025-recorte-dados.md` — trava de treinamento e dado inferido como referência;
- `context/cnn-indice-de-enderecamento.md` — CNN art. 98 e fronteira do acesso;
- `context/travas-defasagem.md` — limites normativos;
- `regime-de-ia-da-uf`, `inventario-lgpd-e-incidentes` e `plano-de-metadados`.

## Autorização e limite

O Provimento CNJ 213/2026, Anexo II, item 3, VI, admite soluções tecnológicas equivalentes, inclusive automação avançada ou IA, para monitoramento e trilhas, desde que preservem **imutabilidade, rastreabilidade e retenção mínima**. Isso não é autorização genérica para decidir, redigir ato ou exportar acervo.

Usar IA para **encontrar e auxiliar conferência**, nunca para qualificar ou decidir sozinha. A solução aponta a fonte; a pessoa autorizada confere o documento original e assume a decisão.

## Arquitetura local por padrão

1. Processar no ambiente controlado da serventia, com chaves sob domínio da própria serventia.
2. Indexar somente o necessário, com identificador persistente e referência ao original.
3. Registrar usuário, data, hora, consulta, filtros, fontes retornadas e ação subsequente.
4. Proteger logs contra alteração e conservá-los pelo mínimo normativo.
5. Impedir retenção, compartilhamento e treinamento pelo fornecedor.
6. Permitir extração integral de índices, metadados, configurações e histórico em formato não proprietário.

Embeddings são zona cinzenta: não declarar que anonimização, reversibilidade ou ausência de memorização estão resolvidas por definição. Expor o risco, documentar a avaliação e manter o padrão local. Dado inferido recebe a mesma trava de não treinamento.

## Os dois acervos

- **Administrativo:** permitir busca e sumarização local compatíveis com finalidade e acesso.
- **Fé pública:** permitir localização e leitura assistida, mas bloquear exportação autônoma, resposta conclusiva e qualquer aparência de certidão, traslado, escritura, ata ou procuração.

Toda saída de acesso administrativo deve informar que não é documento dotado de fé pública e não substitui certidão. Resposta deve trazer identificadores das fontes e nível de confiança, não linguagem de autenticação.

## UF e contratação

Consultar primeiro `regime-de-ia-da-uf`. Nunca transportar autorização de PI ou MA para MT, que proíbe usos, nem tratar AM como operacionalmente endereçável enquanto faltar homologação prévia. Nas demais UFs, aplicar apenas a régua federal confirmada.

Exigir cláusulas de não treinamento, não retenção, confidencialidade, auditoria, reversibilidade, portabilidade e resposta a incidentes. Nada gerado pelo plugin pode ficar preso a ele.

## Saída

Entregar caso de uso, camada, fontes, fluxo humano, arquitetura local, controles, logs, retenção, risco de embeddings, contrato, teste de fuga e bloqueios. Rotular cada função como permitida, condicionada, proibida ou não confirmada.

## Reprovação automática

- enviar acervo identificável a modelo externo;
- usar entrada, saída ou inferência em treinamento;
- permitir que resultado pareça ato ou substitua certidão;
- decidir qualificação automaticamente;
- declarar embeddings seguros por presunção;
- ignorar a UF ou transportar regime entre estados;
- criar dependência do fornecedor ou do plugin.
