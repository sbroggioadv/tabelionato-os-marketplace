---
name: gates-de-partida-e-prazos-de-adequacao
description: "Monta o plano de adequação por classe e os gates estaduais que impedem iniciar IA, combinando os prazos federais de 180, 240 e 300 dias e 24, 30 e 36 meses com autorização de interino no MT e homologação prévia no AM. Esta skill deve ser usada quando o pedido mencionar plano de adequação, cronograma do Provimento 213/2026, art. 20 ou 23, classe de serventia, prazo inicial, prazo global, usar IA em serventia vaga, autorização da CGJ ou homologação no Amazonas."
---

# Gates de partida e prazos de adequação

> Camada C6. Separar autorização para iniciar IA do cronograma federal de TIC; prazo de adequação não suspende vedação imediata.

## Anexos e skills obrigatórios

- `context/prov-cnj-213-2026-e-anexos.md` — classes, etapas, parâmetros e prazos;
- `context/ia-por-uf.md` — gates de MT e AM;
- `context/travas-defasagem.md` — datas não confirmadas e grandezas sem número;
- `diagnostico-de-conformidade-de-ia`, `regime-de-ia-da-uf` e `perfil-da-serventia`.

## Entradas bloqueantes

Confirmar UF, classe vigente, base documental do enquadramento, situação provida ou interina, solução, versão, estágio de uso, data de entrada em vigor aplicável e etapas já comprovadas. Não calcular data-limite sem marco de vigência confirmado.

## Gates estaduais de partida

### MT — serventia vaga e transição

Para interino em serventia vaga, exigir autorização prévia da CGJ antes de contratar ou usar IA, com justificativa técnica, plano de governança, valor compatível com o mercado e parecer do interino, conforme art. 9º. Para solução já usada na entrada em vigor da norma, documentar o regime transitório de **90 dias** do art. 17, sem permitir durante a transição função vedada pelo art. 4º ou risco relevante.

### AM — homologação prévia

Aplicar art. 168, IV, “a”: modelo não homologado previamente pela Corregedoria não pode ser usado. O procedimento público de homologação não foi localizado na data de corte; classificar como **bloqueado / não endereçável**, orientar consulta à CGJ/AM e não declarar ferramenta homologada.

### PI, MA e outras 23 UFs

Aplicar gates locais comprovados em PI e MA sem importar MT ou AM. Nas outras 23 UFs, o silêncio estadual não autoriza função de IA; aplicar o piso federal e tratar os artefatos estaduais como boa prática. A Resolução 615/2025 não cria gate direto para a serventia.

## Cronograma federal por classe

Contar os dois marcos da entrada em vigor do Provimento CN 243/2026, somente após confirmá-la:

| Entrega | Classe 3 | Classe 2 | Classe 1 | Base |
|---|---:|---:|---:|---|
| Etapas 1 e 2, implementação inicial | 180 dias | 240 dias | 300 dias | art. 20 |
| Etapas 1 a 5, implementação integral | 24 meses | 30 meses | 36 meses | art. 23 |

Tratar o prazo inicial como parte integrante do global, não como período adicional. Respeitar a ordem sequencial das etapas e não declarar etapa posterior concluída sem comprovação da anterior. A vigência exata do Provimento 243/2026 não está confirmada no corpus; informar durações, não datas finais inventadas.

## Marcos técnicos do plano

Incluir no cronograma, conforme a classe:

| Controle | Classe 3 | Classe 2 | Classe 1 |
|---|---:|---:|---:|
| RPO máximo | 4 h | 12 h | 24 h |
| RTO máximo | 8 h | 24 h | 24 h |
| backup completo | 24 h | 48 h | 72 h |
| extração integral simulada | 24 meses | 30 meses | 36 meses |

Planejar no mínimo **2 ambientes de backup tecnicamente independentes**, trilhas por **5 anos** e comunicação de incidente crítico em **72 horas**. Não definir retenção do backup nem número de cópias: a norma não os fixa.

## Estrutura do plano

1. classificar a serventia e guardar evidência;
2. mapear Etapas 1 a 5 e dependências;
3. listar requisito, dispositivo, evidência atual, gap e responsável;
4. priorizar gates imediatos, segurança mínima e riscos ao acervo;
5. associar entregas aos prazos inicial e global;
6. programar testes de restauração, extração e auditoria;
7. prever reavaliação anual de classe e mudança de fornecedor;
8. registrar conclusão somente com dossiê ou relatório simplificado cabível.

Não usar o cronograma para adiar mitigação mínima já exigível ou função estadual proibida.

## Saída

Entregar decisão de partida, classe e evidência, cronograma por etapa, matriz de controles, prazos em duração, gaps, responsáveis, dependências, testes e declaração de limitações. Separar `pode iniciar IA` de `está em adequação TIC`.

## Reprovação automática

- autorizar interino no MT sem CGJ;
- autorizar IA no AM sem homologação comprovada;
- somar prazo inicial ao global;
- trocar as classes ou os números;
- calcular data final sem vigência confirmada;
- fixar retenção do backup;
- usar prazo de adequação para manter função proibida;
- declarar etapa concluída sem evidência.
