---
name: plano-de-metadados
description: "Estrutura o plano de metadados do acervo com os 13 campos do Anexo II do Decreto 10.278/2020, vocabulário controlado, identificador e hash, sem transformar nome de arquivo em falsa norma. Esta skill deve ser usada quando o pedido mencionar indexação, metadados, taxonomia, identificador, hash, classificação, busca, migração, arquivo estruturado ou padrão de nome de arquivo."
---

# Plano de metadados

## Três invioláveis

1. Nada do acervo sai sem anonimização irreversível prévia.
2. Nada alimenta treinamento: nem entrada, nem saída, nem dado inferido.
3. Nada produzido pelo plugin é ato notarial ou registral nem pode parecer ato dotado de fé pública.

Aplicar **IMUTABILIDADE, RASTREABILIDADE e RETENÇÃO MÍNIMA** em toda automação. Base normativa atualizada até 25/08/2026.

Tratar o acervo como patrimônio funcional **do serviço**, não do titular; tudo que esta skill gerar deve ser extraível em formato não proprietário, sem anuência de fornecedor. Separar a camada administrativa da camada de fé pública: nesta última, leitura autorizada pode ocorrer, mas saída com aparência de ato nunca.

## Anexos e skills obrigatórios

- `context/decreto-10278-2020.md` — Anexo II e requisitos de integridade;
- `context/prov-cnj-213-2026-e-anexos.md` — interoperabilidade e portabilidade;
- `context/cnn-indice-de-enderecamento.md` — Arquivo Eletrônico Estruturado;
- `diagnostico-do-acervo`, `conformidade-de-digitalizacao` e `busca-local-no-acervo-e-a-fronteira`.

## Regra central

O padrão nacional é de **metadados**, não de nomenclatura de arquivos. Não apresentar máscara de nome, sequência de pastas ou convenção interna como obrigação normativa. Nomes podem facilitar operação, mas a identidade, a prova e a busca vivem nos campos estruturados.

## Os oito metadados para todo documento

Implementar exatamente os campos do Anexo II do Decreto 10.278/2020:

1. **Assunto** — palavras-chave com vocabulário controlado;
2. **Autor (nome)**;
3. **Data e local da digitalização**;
4. **Identificador do documento digital** — único e persistente;
5. **Responsável pela digitalização**;
6. **Título**;
7. **Tipo documental**;
8. **Hash (checksum) da imagem**.

Não colocar dado pessoal desnecessário em título, assunto, caminho ou nome de arquivo. O hash verifica integridade; não substitui assinatura, cadeia de custódia nem trilha de auditoria.

## Os cinco metadados adicionais

Quando aplicável o bloco do Anexo II para documentos digitalizados por pessoa jurídica de direito público interno, acrescentar:

9. **Classe**;
10. **Data de produção do original**;
11. **Destinação prevista** — eliminação ou guarda permanente;
12. **Gênero**;
13. **Prazo de guarda**.

Não presumir que a serventia delegada se converte em pessoa jurídica de direito público. Manter os cinco campos como perfil estendido recomendado para interoperabilidade e temporalidade, distinguindo obrigação diretamente aplicável de adoção conservadora.

## Modelo de governança

Definir para cada campo: nome canônico, finalidade, tipo, formato, domínio permitido, obrigatoriedade, origem, responsável, regra de validação, versionamento e histórico de alterações. Manter dicionário e vocabulário controlado versionados, com sinônimos redirecionados ao termo preferido.

Vincular cada registro ao conjunto do diagnóstico e à camada correspondente:

- **administrativa:** pode sustentar filtros e automações locais autorizadas;
- **fé pública:** permite localização e conferência, mas nenhuma saída automática se torna traslado, certidão ou ato.

Exportar metadados em formato interoperável e não proprietário. Preservar identificadores e hashes em migrações, com relatório de correspondência antes/depois.

## Controles de qualidade

- rejeitar identificador duplicado, campo obrigatório vazio e hash ausente quando houver imagem;
- validar datas, domínio do tipo documental e destinação contra a tabela de temporalidade;
- impedir que “eliminação” seja atribuída a livro permanente;
- registrar versão do esquema e autor da alteração;
- testar busca por identificador, assunto, tipo, data e destinação;
- separar falha de metadado de falha no documento de origem.

## Saída

Entregar dicionário dos 13 campos, perfil mínimo e estendido, vocabulário controlado, regras de validação, esquema de exportação, plano de migração e relatório de lacunas. Rotular convenções internas de nome como internas, nunca como norma nacional.

## Reprovação automática

- omitir um dos 13 campos;
- inventar padrão nacional de nome de arquivo;
- usar hash como sinônimo de assinatura;
- guardar PII desnecessária em nomes ou caminhos;
- prender metadados a formato proprietário;
- permitir que saída de busca pareça documento dotado de fé pública.
