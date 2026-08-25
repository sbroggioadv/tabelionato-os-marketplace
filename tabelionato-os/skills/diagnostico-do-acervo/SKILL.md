---
name: diagnostico-do-acervo
description: "Inventaria o acervo da serventia por suporte, camada, estado de conservação, prazo de guarda, proteção e possibilidade legal de eliminação, preservando a continuidade do serviço e a transferência ao sucessor. Esta skill deve ser usada quando o pedido mencionar diagnóstico, inventário, migração, organização, legado, papel, livro, documento digital, acervo administrativo ou acervo de fé pública."
---

# Diagnóstico do acervo

## Três invioláveis

1. Nada do acervo sai sem anonimização irreversível prévia.
2. Nada alimenta treinamento: nem entrada, nem saída, nem dado inferido.
3. Nada produzido pelo plugin é ato notarial ou registral nem pode parecer ato dotado de fé pública.

Aplicar **IMUTABILIDADE, RASTREABILIDADE e RETENÇÃO MÍNIMA** em toda automação. Base normativa atualizada até 25/08/2026.

Tratar o acervo como patrimônio funcional **do serviço**, não do titular; tudo que esta skill gerar deve ser extraível em formato não proprietário, sem anuência de fornecedor. Separar a camada administrativa da camada de fé pública: nesta última, leitura autorizada pode ocorrer, mas saída com aparência de ato nunca.

## Anexos e skills obrigatórios

- `context/lei-8935-94.md` — dever de ordem, busca, guarda e conservação;
- `context/prov-cnj-50-2015-temporalidade-notas.md` — classes e prazos de guarda;
- `context/prov-cnj-213-2026-e-anexos.md` — proteção, continuidade e transferência ao sucessor;
- `context/travas-defasagem.md` — descarte, incidentes e prova defensiva;
- `temporalidade-e-eliminacao`, `inventario-lgpd-e-incidentes` e `teste-de-extracao-integral-e-portabilidade`.

## Premissa de titularidade

Tratar o acervo como patrimônio funcional **do serviço**, nunca como ativo pessoal do titular. A Lei 8.935/1994, art. 46, atribui guarda e responsabilidade; não propriedade. O Provimento CNJ 213/2026, art. 6º, III, exige transferência organizada ao sucessor, incluindo bases, softwares, manuais, políticas, acessos, ativos e histórico de atualizações.

## Separar os dois acervos

1. **Camada administrativa:** gestão, contratos, pessoas, fornecedores, contabilidade, inventário de dados, segurança e rotinas internas. É o terreno possível de automação, sob finalidade, minimização e controle.
2. **Camada de fé pública:** livros, atos, imagens, índices e dados próprios do acervo notarial ou registral. Pode ser lida localmente para busca autorizada; não pode gerar saída que se apresente como certidão, traslado ou ato.

Não fundir as camadas. O direito de acesso administrativo do CNN art. 98 não alcança os dados próprios do acervo de fé pública.

## Inventário operacional

Para cada conjunto documental, registrar:

- função, espécie documental, período, volume e responsável pela custódia;
- suporte: livro físico, papel avulso, microfilme, imagem, PDF/A, XML, base estruturada, log ou backup;
- camada administrativa ou de fé pública, grau de sigilo e presença de dados pessoais;
- sistema e fornecedor, formato, chave de acesso, localização, cópias e dependências;
- regra de guarda, termo inicial, prazo, evento de descarte e fonte normativa;
- integridade verificável, hash quando cabível, trilha de auditoria e capacidade de busca;
- estado de conservação, risco de perda, indisponibilidade, obsolescência ou aprisionamento tecnológico;
- capacidade de extração integral em formato interoperável e não proprietário.

Classificar a evidência como confirmada, pendente ou não localizada. Não estimar volumes, prazos nem conformidade.

## Regras de decisão

- Manter todos os livros de notas permanentemente, inclusive quando digitalizados.
- Só marcar papel como eliminável após prazo cumprido, digitalização com valor legal quando exigida e validação da tabela aplicável.
- Separar eliminação física de retenção dos índices, classificadores, backups e dados remanescentes sob LGPD.
- Não remover documentos para perícia: o art. 46, parágrafo único, determina exame na sede, com ciência do titular e autorização do juízo.
- Não recomendar solução proprietária sem saída autônoma; nada gerado pelo plugin pode ficar preso ao plugin ou exigir anuência do fornecedor para migração.

## Saída

Entregar matriz do acervo, mapa dos dois domínios, riscos por conjunto, prazos e fontes, fila de digitalização, fila de descarte condicionada, lacunas de integridade e plano de transferência ao sucessor. Identificar claramente o que **não pode ser eliminado** e o que ainda depende de confirmação humana ou normativa.

## Reprovação automática

- chamar o acervo de bem do titular;
- permitir saída de dado identificável ou uso para treinamento;
- tratar busca administrativa como emissão de documento de fé pública;
- propor eliminação de livro de notas;
- inventar prazo de guarda;
- aceitar formato proprietário ou migração dependente do fornecedor.
