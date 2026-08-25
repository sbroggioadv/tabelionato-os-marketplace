---
name: tabelionato-onboarding
description: "Onboarding sem PII do tabelionato-os. Coleta por escolhas fechadas a UF, classe de receita bruta semestral do Provimento 213/2026, atribuições da serventia, uso atual de IA e situação provida ou vaga/interina; grava somente o perfil institucional e a data de corte do contexto. Esta skill deve ser usada na primeira sessão, quando não houver perfil, ao reconfigurar a serventia ou quando o pedido mencionar /start, começar, configurar tabelionato, onboarding, classe da serventia, já usa IA, ofício único, interino ou atualizar perfil."
---

# Tabelionato Onboarding — `/start`

> Camada C0. Configurar a **serventia**, não um caso. Não colher dados de parte, cliente, ato ou acervo.

## Anexos obrigatórios

- `context/estado-da-norma.md` — data de corte a persistir;
- `context/uf-matriz-27.md` — 27 UFs e autoridades;
- `context/prov-cnj-213-2026-e-anexos.md` — classes do art. 16, na redação do Provimento CN 243/2026;
- `context/ia-por-uf.md` — regimes estaduais de IA.

## Ferramenta e estilo

Usar `AskUserQuestion` em toda lista fechada, com botões. Dividir listas longas em perguntas sucessivas. Fazer uma pergunta por vez e confirmar o resumo antes de gravar.

## Perguntas obrigatórias

### 1. UF

Perguntar primeiro a região e depois a UF:

- Norte: AC, AP, AM, PA, RO, RR, TO;
- Nordeste: AL, BA, CE, MA, PB, PE, PI, RN, SE;
- Centro-Oeste: DF, GO, MT, MS;
- Sudeste: ES, MG, RJ, SP;
- Sul: PR, RS, SC.

Não aceitar “Brasil” como perfil suficiente. A UF governa rito, prazo, órgão, IA e emolumentos.

### 2. Classe tecnológica

Explicar que a classe usa **receita bruta semestral**, não valor de ato nem renda pessoal. Oferecer:

- **Classe 1:** receita bruta semestral de até R$ 300.000;
- **Classe 2:** acima da Classe 1 e até R$ 1.500.000 de receita bruta semestral;
- **Classe 3:** acima do limite da Classe 2;
- **Não sei:** encaminhar para conferência contábil sem guardar números.

Não perguntar receita exata. Persistir apenas `classe_1`, `classe_2`, `classe_3` ou `nao_confirmada`.

### 3. Atribuições

Oferecer:

- Tabelionato de Notas isolado;
- Ofício único com Notas e outras atribuições;
- Notas acumulado com atribuição específica;
- Estrutura ainda não confirmada.

Na acumulação, permitir marcar as atribuições por categoria institucional, sem dados de usuários.

### 4. Uso atual de IA

Oferecer:

- Não usa;
- Avalia fornecedores;
- Piloto controlado;
- Uso em produção;
- Situação não confirmada.

Registrar somente o estágio. Não colher nome de fornecedor, contrato, prompts, documentos, base ou conteúdo do acervo. Se a UF não for PI, MT, MA ou AM, explicar que a ausência de norma estadual localizada não elimina os deveres federais nem futura atualização.

### 5. Situação da delegação

Oferecer:

- Serventia provida por titular;
- Serventia vaga com interino/responsável;
- Situação em transição;
- Não confirmada.

Essa resposta altera gates de IA e governança, especialmente autorizações dirigidas a serventia vaga/interino.

## Confirmação e persistência

Exibir a ficha sem PII:

```yaml
uf: XX
classe_tic: classe_1 | classe_2 | classe_3 | nao_confirmada
atribuicoes: [notas_isolado | oficio_unico | acumulada | nao_confirmada]
uso_ia: nao_usa | avaliacao | piloto | producao | nao_confirmado
situacao_delegacao: provida | vaga_interino | transicao | nao_confirmada
data_corte_contexto: 25/08/2026
```

Solicitar confirmação por botão e entregar a ficha a `perfil-da-serventia`. Se já existir perfil, oferecer **Atualizar** ou **Manter**; não apagar silenciosamente campos confirmados.

## Explicação final

Informar em linguagem simples:

1. toda demanda começa por UF e modalidade presencial/eletrônica;
2. a classe altera requisitos de TIC e acervo;
3. uso de IA depende do piso federal e, quando houver, da norma estadual;
4. o plugin verifica e documenta, mas não decide pelo titular;
5. a base tem data de corte em 25/08/2026 e precisa de atualização para afirmar vigência posterior.

## Entrega obrigatória

Entregar resumo de cinco campos, data de corte e handoff para `tabelionato-master`. Não produzir minuta, parecer sobre ato ou valor de emolumento.

## Guard de privacidade

Nunca perguntar ou persistir nome, CPF/CNPJ, e-mail, telefone, endereço, matrícula funcional, número de delegação, dados de parte/cliente, documento, ato, protocolo, conteúdo de livro, acervo ou fornecedor. Descrever a serventia por categorias institucionais.
