---
name: diagnostico-de-conformidade-de-ia
description: "Mapeia a conformidade de IA aplicável à serventia por UF, classe TIC, solução, uso e situação da delegação, separando piso federal, obrigação estadual e boa prática antecipatória. Esta skill deve ser usada quando o pedido mencionar diagnóstico de IA, conformidade do cartório, quais normas se aplicam, classe 1, 2 ou 3, receita bruta semestral, RPO, RTO, backup, logs, prazo de adequação, Resolução 615/2025 ou mapa de obrigações para a Corregedoria."
---

# Diagnóstico de conformidade de IA

> Camada C6. Mapear o que se aplica e gerar evidência; não certificar conformidade nem substituir parecer jurídico ou técnico.

## Anexos e skills obrigatórios

- `context/ia-por-uf.md` — quatro regimes estaduais e 23 UFs sem norma localizada;
- `context/prov-cnj-213-2026-e-anexos.md` — piso federal de TIC, acervo e classes;
- `context/res-cnj-615-2025-recorte-dados.md` — referência de governança, sem vínculo próprio da serventia;
- `context/travas-defasagem.md` — números confirmados, lacunas e remissões mortas;
- `perfil-da-serventia`, `regime-de-ia-da-uf` e `varredura-de-vigencia-pre-lavratura`.

## Entradas bloqueantes

Fixar UF, classe TIC ou receita bruta semestral documentada, solução e versão, fornecedor, finalidade, dados processados, arquitetura, estágio de uso, situação provida ou interina e data do diagnóstico. Não armazenar receita exata no perfil institucional nem inserir dado de parte ou acervo em ferramenta externa.

## Honestidade de escopo

Declarar obrigatoriamente:

- somente **PI, MT, MA e AM** possuíam norma estadual de IA localizada na data de corte de 25/08/2026;
- nas outras **23 UFs**, aplicar apenas o piso federal de TIC, proteção de dados e acervo; os artefatos estaduais podem ser oferecidos somente como boa prática antecipatória, não como obrigação local;
- a Resolução CNJ 615/2025 rege o Poder Judiciário e **não vincula a serventia por força própria**; utilizá-la apenas quando norma estadual remeter a ela ou como referência não obrigatória;
- o Provimento CN 213/2026 não é norma estadual de autorização de usos de IA: é piso federal de TIC e proteção do acervo.

## Classificação por receita bruta semestral

Aplicar o Provimento CN 213/2026, art. 16, na redação do Provimento 243/2026:

| Classe | Receita bruta semestral |
|---|---:|
| 1 | até R$ 300.000,00 |
| 2 | acima de R$ 300.000,00 e até R$ 1.500.000,00 |
| 3 | acima de R$ 1.500.000,00 |

Calcular a receita pelo art. 2º, XXIV: incluir emolumentos, outras receitas, ressarcimento de gratuitos e renda mínima; deduzir somente valores de terceiros e repasses legais obrigatórios. Não deduzir custeio, pessoal, investimento ou tributos do delegatário.

Reavaliar anualmente pela média das receitas brutas semestrais do exercício anterior. Verificar atualização anual dos limites e a regra de estabilização de 10% por dois ciclos antes de concluir migração de classe.

## Matriz técnica obrigatória

| Requisito | Classe 3 | Classe 2 | Classe 1 |
|---|---:|---:|---:|
| RPO máximo | 4 h | 12 h | 24 h |
| RTO máximo | 8 h | 24 h | 24 h |
| backup completo, intervalo máximo | 24 h | 48 h | 72 h |
| simulação de extração integral | 24 meses | 30 meses | 36 meses |

Exigir no mínimo **2 ambientes de backup tecnicamente independentes**, com ao menos um protegido contra comprometimento simultâneo. Exigir retenção das trilhas de auditoria por **5 anos** e comunicação de incidente crítico à Corregedoria em até **72 horas**.

Não fixar retenção do próprio backup: a norma não determina esse prazo. Não converter os 2 ambientes em quantidade de cópias ou gerações. Não tratar as bandas referenciais como velocidade obrigatória quando testes documentados provarem o atendimento funcional.

## Mapa dos oito artefatos

Classificar cada entrega como `obrigatória`, `boa_prática_antecipatória`, `bloqueada` ou `não_aplicável`:

1. análise prévia de risco;
2. avaliação de impacto e RIPD;
3. cláusulas do fornecedor;
4. comunicação anual;
5. registro interno de usos;
6. capacitação;
7. classificação e parâmetros técnicos;
8. plano de adequação e gates de partida.

Vincular cada linha ao dispositivo federal e, quando houver, estadual. No AM, manter bloqueio de uso sem homologação prévia comprovada. No MT, não permitir função proibida mesmo sob revisão humana.

## Saída

Entregar cartão com UF, postura estadual, classe e base de cálculo, solução, finalidade, artefatos aplicáveis, matriz técnica, gaps, prazos sem data inventada, evidências disponíveis e próximos responsáveis. Marcar toda conclusão como diagnóstico documental, não certificado de conformidade.

## Reprovação automática

- dizer que 27 UFs regularam IA;
- aplicar obrigação estadual às outras 23 UFs;
- tratar a Resolução 615/2025 como vinculante por força própria;
- confundir classe TIC com emolumento ou faturamento mensal;
- trocar a ordem C3/C2/C1 dos parâmetros;
- fixar retenção de backup;
- autorizar IA no AM sem homologação;
- emitir selo ou certificação de conformidade.
