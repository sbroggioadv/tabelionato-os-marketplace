---
name: classificacao-por-classe-e-plano-de-tic
description: "Classifica a serventia pela receita bruta semestral e converte a Classe 1, 2 ou 3 em plano de TIC com RPO, RTO, backup, logs, incidentes, testes e prazos do Provimento CNJ 213/2026. Esta skill deve ser usada quando o pedido mencionar classe da serventia, receita, infraestrutura, continuidade, backup, RPO, RTO, log, vulnerabilidade, pentest ou plano de adequação tecnológica."
---

# Classificação por classe e plano de TIC

## Três invioláveis

1. Nada do acervo sai sem anonimização irreversível prévia.
2. Nada alimenta treinamento: nem entrada, nem saída, nem dado inferido.
3. Nada produzido pelo plugin é ato notarial ou registral nem pode parecer ato dotado de fé pública.

Aplicar **IMUTABILIDADE, RASTREABILIDADE e RETENÇÃO MÍNIMA** em toda automação. Base normativa atualizada até 25/08/2026.

Tratar o acervo como patrimônio funcional **do serviço**, não do titular; tudo que esta skill gerar deve ser extraível em formato não proprietário, sem anuência de fornecedor. Separar a camada administrativa da camada de fé pública: nesta última, leitura autorizada pode ocorrer, mas saída com aparência de ato nunca.

## Anexos e skills obrigatórios

- `context/prov-cnj-213-2026-e-anexos.md` — classes, controles, etapas e prazos;
- `context/travas-defasagem.md` — números duros e obrigações periódicas;
- `perfil-da-serventia`, `teste-de-extracao-integral-e-portabilidade` e `inventario-lgpd-e-incidentes`.

## Entrada e classificação

Usar **receita bruta semestral**, nunca emolumento isolado, receita mensal ou valor líquido:

- **Classe 1:** até R$ 300.000,00;
- **Classe 2:** acima de R$ 300.000,00 e até R$ 1.500.000,00;
- **Classe 3:** acima de R$ 1.500.000,00.

Aplicar as dez subclasses do art. 16 do Provimento CNJ 213/2026, na redação do Provimento CN 243/2026, quando houver receita exata, sem alterar a classe principal. Não estimar a classe; se o dado não existir, emitir quadro das três possibilidades.

## Matriz obrigatória

| Controle | Classe 3 | Classe 2 | Classe 1 |
|---|---:|---:|---:|
| RPO máximo | 4 h | 12 h | 24 h |
| RTO máximo | 8 h | 24 h | 24 h |
| intervalo máximo de backup completo | 24 h | 48 h | 72 h |
| teste de restauração | semestral | anual | anual |
| simulação de extração integral | 24 meses | 30 meses | 36 meses |
| prazo inicial do art. 20 | 180 dias | 240 dias | 300 dias |
| horizonte global do art. 23 | 24 meses | 30 meses | 36 meses |

Em todas as classes: manter backups em pelo menos **dois ambientes tecnicamente independentes**; trilhas de auditoria por pelo menos **cinco anos**; comunicar incidente crítico à Corregedoria em até **72 horas**; tratar vulnerabilidade crítica em até **30 dias** quando não houver exploração ativa e adotar contenção imediata se houver exploração ou risco iminente.

Para Classe 3, prever pentest ou equivalente no mínimo a cada dois anos e nos eventos normativos, observando as hipóteses de relatório coletivo ou dispensa condicionada em SaaS. Não transformar banda de 2/10/50 Mbps em mínimo absoluto: a própria norma a trata como referencial e exige prova de atendimento ao RPO.

## Plano por evidência

Para cada controle, registrar situação atual, lacuna, responsável, ação, prazo normativo, dependência, evidência de conclusão e risco residual. Organizar por continuidade, recuperação, segurança, logs, vulnerabilidades, interoperabilidade e governança.

O plano deve garantir transferência organizada ao sucessor e exportação em formato interoperável e não proprietário. Nada gerado pelo plugin pode criar dependência do plugin.

## Silêncio normativo obrigatório

O Provimento 213 disciplina periodicidade e arquitetura de backup, mas **não fixa retenção do backup em si**. Não inventar dias, meses ou anos. Distinguir sempre retenção de logs, que é de cinco anos, da retenção das cópias de segurança.

Não calcular datas-limite dos arts. 20 e 23 sem data de vigência confirmada do texto aplicável; informar duração e termo inicial pendente.

## Saída

Entregar classe e subclasse, memória de cálculo, matriz de controles, lacunas, cronograma por etapa, evidências, riscos e pontos pendentes. Se faltar receita ou vigência, emitir cenários sem escolher silenciosamente.

## Reprovação automática

- classificar por receita mensal ou líquida;
- trocar a ordem C3/C2/C1 dos números;
- fixar retenção de backup;
- tratar banda referencial como requisito absoluto;
- omitir dois ambientes, logs de cinco anos ou incidente crítico em 72 horas;
- prender continuidade ou extração a fornecedor.
