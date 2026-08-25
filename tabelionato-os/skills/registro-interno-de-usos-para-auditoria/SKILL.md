---
name: registro-interno-de-usos-para-auditoria
description: "Define política de registro interno e logs de usos de IA para auditoria, distinguindo o formato ainda não definido do MT, o registro de todas as interações no AM e a retenção federal de trilhas por 5 anos. Esta skill deve ser usada quando o pedido mencionar log de IA, registro de prompts, trilha de auditoria, usuário, timestamp, resultado gerado, Corregedoria pedir logs, retenção de 5 anos, imutabilidade, rastreabilidade ou política interna de uso de IA."
---

# Registro interno de usos para auditoria

> Camada C6. Registrar o necessário para reconstruir uso e responsabilidade sem transformar o log em segunda cópia do acervo.

## Anexos e skills obrigatórios

- `context/ia-por-uf.md` — regras de MT e AM;
- `context/prov-cnj-213-2026-e-anexos.md` — trilhas, integridade e retenção;
- `context/travas-defasagem.md` — forma indefinida no MT e prazo federal;
- `regime-de-ia-da-uf`, `diagnostico-de-conformidade-de-ia` e `comunicacao-anual-a-corregedoria`.

## Honestidade de escopo

Aplicar as regras estaduais somente onde existem:

- **MT art. 6º, VI:** registrar utilizações relevantes ou representativas para auditoria e fiscalização, na forma ainda a ser definida pela CGJ; não inventar formulário, campos obrigatórios ou carga de registro total;
- **AM art. 166, IV:** registrar logs detalhados de **todas as interações**, incluindo usuário, timestamp, ações e resultados gerados, além de rastreabilidade sequencial;
- **PI:** assegurar transparência e auditabilidade do sistema, sem atribuir ao art. 103 um formato local de log não escrito;
- **MA arts. 176-177:** garantir auditabilidade e relatórios técnicos, sem inventar retenção estadual própria.

Nas outras 23 UFs, aplicar o piso federal de trilhas de auditoria. A Resolução CNJ 615/2025 permanece referência sem vínculo próprio da serventia.

## Esquema mínimo seguro

Registrar por evento, conforme o regime aplicável:

- identificador imutável do evento;
- identidade funcional ou pseudonimizada do usuário autorizado;
- data e hora sincronizadas;
- solução, versão e função usada;
- categoria da ação e finalidade;
- classe de dado, nunca o conteúdo integral;
- indicador de anonimização e ambiente;
- identificador criptográfico ou referência controlada da entrada e saída, sem replicá-las quando contiverem acervo;
- resultado operacional, revisão humana, correção e responsável;
- incidente, bloqueio ou exceção;
- vínculo com contrato, risco, impacto e comunicação.

No AM, atender o requisito de ações e resultados gerados sem expor dado confidencial: armazenar o conteúdo somente em ambiente autorizado e protegido quando indispensável; preferir hash, referência e metadados quando bastarem à reconstrução.

## Controles da trilha

Garantir integridade verificável, proteção contra alteração, acesso restrito, sincronização de tempo, segregação, exportação auditável e integração com backup e recuperação. Reter as trilhas de auditoria por no mínimo **5 anos**, conforme Anexo II do Provimento 213/2026, admitido prazo superior com base própria.

Não confundir retenção de log com retenção de backup. A norma **não fixa por quanto tempo guardar o próprio backup**; permanecer calado sobre esse prazo e consultar temporalidade e exigência específica.

## Acesso e fiscalização

Permitir extração controlada para a Corregedoria competente, com escopo, período, cadeia de custódia, minimização e registro do próprio acesso. No MT, reconhecer que a CGJ pode solicitar relatórios, logs ou documentos a qualquer tempo, sem preencher a lacuna sobre a forma futura.

## Saída

Entregar política interna, dicionário de campos, matriz de acesso, regra de retenção, fluxo de exportação, controles de integridade, teste de reconstrução e lacunas estaduais. Não criar log contendo credencial, chave, dado pessoal ou inteiro teor do acervo por padrão.

## Reprovação automática

- inventar a forma ainda não definida do MT;
- registrar apenas usos relevantes no AM;
- omitir usuário, timestamp, ação ou resultado no AM;
- guardar conteúdo de acervo indiscriminadamente;
- permitir alteração sem trilha;
- reter logs por menos de 5 anos;
- afirmar prazo de retenção do backup;
- aplicar a Resolução 615 diretamente à serventia.
