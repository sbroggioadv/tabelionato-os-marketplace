# Travas de defasagem — dossiê consolidado do `tabelionato-os`

> **Data de corte normativa e jurisprudencial: 25/08/2026.** Este anexo preserva integralmente as travas T-01 a T-132 consolidadas das nove frentes; qualquer uso posterior exige a rotina de atualização e os gates de vigência descritos aqui.

> **Fan-in das 5 frentes de pesquisa dedicada** (F1 a F5, todas conduzidas em 25/08/2026) sobre a
> `PESQUISA-META.md` de 18/08/2026. Consolidação escrita em **25/08/2026**.
>
> **Isto é insumo de decisão, não decisão.** Nenhum DESIGN-SPEC, PRD ou build nasce daqui. Nenhuma
> afirmação abaixo é minha: tudo é rastreável a uma das cinco frentes, com a frente de origem
> nomeada. Onde duas frentes se contradizem e a fonte não resolve, está dito com todas as letras.
>
> **Selos preservados das frentes:** ✅ verificado em fonte primária · 🟡 plausível / fonte
> secundária / inferência declarada · 🔴 não confirmado. **Nenhum 🟡 foi promovido a ✅ nesta
> consolidação.**
>
> **Fontes desta consolidação:** `_planning/novas-verticais/tabelionato/PESQUISA-META.md` ·
> `pesquisa/F1-codigo-nacional-normas.md` · `pesquisa/F2-atos-notariais.md` ·
> `pesquisa/F3-desjudicializacao.md` · `pesquisa/F4-responsabilidade-pad.md` (**revisão 2**) ·
> `pesquisa/F5-mercado-emolumentos.md` · capturas verbatim em `pesquisa/capturas/`.

---

## 0. Premissas cravadas pelo Doc (25/08/2026) — não são mais pergunta

Três botões foram respondidos **depois** das cinco frentes. Deixam de ser decisão aberta e passam a
ser **premissa** deste dossiê. A seção 9 traz apenas o que continua genuinamente em aberto.

| # | Decisão | Onde ela reescreve este dossiê |
|---|---|---|
| **P-1** | **A camada de conformidade regulatória de IA ENTRA no v0.1, como diferencial CENTRAL** — não como apêndice | §2.2-bis (camada de primeira classe, com os 6 artefatos) e §5.5 (a fragilidade que o produto tem de declarar: **só MT regulou**) |
| **P-2** | **R$ 498, pagamento único**, com "atualizações exclusivas para membros da comunidade IA Combativa" promovida a **argumento central da oferta** | §7.4 fecha no número; §7.6 converte o alerta de envelhecimento da F5 em **requisito de arquitetura**, não em ressalva comercial |
| **P-3** | **Nome `tabelionato-os`** · v0.1 = **Tabelionato de NOTAS isolado**; Registro de Imóveis vira **plugin-irmão ou v0.2** | §2.4 e §2.5 deixam de ser opção e passam a ser recorte fechado |

> **Nota de revisão (25/08/2026):** a **F4 foi revisada** depois da primeira consolidação (45 KB →
> 55 KB), com intel cruzada da F2. Três itens que eu havia consolidado mudaram e foram corrigidos
> aqui: a régua temporal do art. 22 tem **três** faixas, não duas (T-96); a correção sobre
> "responsabilidade subsidiária do Estado" foi **corrigida contra a própria F4** (T-98 e C-18); e as
> travas R16-R18 entraram, enriquecendo T-32, T-42 e T-64. O detalhe de cada correção está marcado
> em cada trava.

---

## 1. Veredito em 10 linhas

1. **A tese central da meta se confirma por dado, não por intuição:** Tabelionato de Notas é a
   atribuição que paga o plugin — **8.228 das 12.210 serventias** (67,4%), 38% da procura do cidadão
   (Datafolha 2025), 2,3 mi de escrituras no e-Notariado. ✅ F5.
2. **Mas a premissa comercial da meta caiu:** o espaço "assistente que redige a minuta" **já está
   ocupado, e pela entidade de classe do próprio comprador** — a **IA Not** do CNB/CF, dentro do
   e-Notariado, desde set/2025, provavelmente gratuita. ✅ F5.
3. **E surgiu uma camada que a meta não viu:** IA dentro de serventia **é objeto de norma** desde
   2026 — Res. CNJ 615/2025, Prov. CNJ 213/2026 e **Prov. TJMT 1/2026**, que **veda nominalmente**
   "qualificação registral" por IA e **autoriza** "minuta preliminar sob revisão humana". ✅ F5.
4. **Duas skills do esqueleto §7.1 estão fora da lei que rege o comprador** — `qualificacao-registral-e-duvida`
   pelo nome e pela promessa (art. 4º, II), e o gate `varredura-...-pre-lavratura` se "decidir" em vez
   de "exibir" (art. 4º, III). É reescrita de posicionamento, não de escopo. ✅ F5.
5. **O corpus notarial não está onde a meta procurou:** o "Livro do Tabelionato de Notas" do CNN é
   residual; o núcleo está na **Parte Geral, Livro IV, Cap. VI, arts. 264-319** (e-Notariado/CENSEC).
   São **4 endereços** distantes — o índice de endereçamento é o primeiro artefato do `context/`. ✅ F1.
6. **A execução extrajudicial de hipoteca não é registral:** a **ata notarial de arrematação** (Lei
   14.711/2023, art. 9º, §11) é do tabelião de notas, tem competência própria, **zero regulamentação
   do CNJ** e é a **única ata desta onda que é título translativo**. Estava na camada errada. ✅ F3.
7. **Não existe "a natureza da responsabilidade notarial" — existe a natureza NA DATA DO ATO**, em
   **três** faixas (a do meio, da Lei 13.137/2015, ninguém tinha registrado); e o triênio conta da
   lavratura **pela letra**, mas o STJ conta do trânsito em julgado da anulatória quando o dano só
   se define ali. ✅ F4 rev. 2.
8. **Três camadas do produto são "nunca hardcodar, sempre conferir o estado", não uma:** emolumentos
   (26 leis estaduais **+ 1 lei federal no DF**), **rito e prescrição do PAD**, e o **procedimento de
   recusa do tabelião de notas** — que não tem equivalente federal. ✅ F2/F4/F5.
9. **A norma operacional muda ~2× por mês** (57 alterações do CNN em 24 meses, 16 só em 2026) e
   **suspensão é rotina** (172, 175 e 247 em 26 meses). Este é o plugin da família em que o pagamento
   único envelhece mais rápido. ✅ F1/F5.
10. **A decisão que a pesquisa pedia, o Doc cravou (P-1):** o eixo do v0.1 é **conformidade
    regulatória de IA como diferencial central**, somada à defesa técnica do titular, ao gate de
    vigência e às obrigações periódicas que ninguém cobre. A redação de minuta continua existindo,
    mas **não é a promessa** — ali o concorrente é o CNB, dentro da plataforma do CNB, de graça.

---

## 2. O que MUDOU no esqueleto (§7.1 da `PESQUISA-META.md`)

Camada por camada. Cada mudança carrega o achado que a motivou e a frente de origem.

### 2.0 Duas mudanças estruturais que atravessam todas as camadas

**(a) A "Camada 1" da meta são duas camadas.** F3 §13.1: "atos de balcão" (escritura, ata,
procuração, testamento) e "procedimentos de desjudicialização" (inventário, divórcio, usucapião,
adjudicação, arrematação, precatório) têm gates diferentes — os procedimentos têm **porta de
entrada** (consulta obrigatória, autorização de CGJ, advogado obrigatório), **interlocutor externo**
(MP, juízo sucessório, registrador, tribunal) e **efeito condicionado** (eficácia dependente do MP,
título dependente de registro). Merecem camada própria.

**(b) A pergunta "presencial ou eletrônico" precede qualquer minuta.** F2 §12.1: ela muda a
competência (absoluta no eletrônico, CNN 289/302-304), os requisitos (CNN 286) e as nulidades (CNN
318 e 319 §1º). Um master que pergunte só "qual ato?" produz minuta eletrônica com fundamento
presencial. A ordem certa é **ato → presencial ou eletrônico → competência → qualificação → minuta**.

### 2.1 Orquestrador e QA

| Item do esqueleto | Veredito | Motivo (frente) |
|---|---|---|
| `tabelionato-master` | **Sobrevive**, com a ordem de perguntas reescrita | A meta previa "identifica especialidade + tipo de ato". Falta o eixo presencial × eletrônico, que é o que muda competência e nulidade — F2 §12.1 ✅ |
| `suprema-corte-tabelionato` R1-R4 | **Sobrevive e muda de objeto** | A meta o desenhou para checar "se o provimento foi absorvido ou está suspenso" — **dois** estados. São **três** (ABSORVIDO · VIVO POR REMISSÃO · SUSPENSO — F1 §6) e mais **três tipos** de provimento (alterador · autônomo · Resolução do Plenário — F3 §1.1). São seis valores a resolver, não dois ✅ |

### 2.2 Camada 0 — Fundação

| Item | Veredito | Motivo (frente) |
|---|---|---|
| `regime-delegatario` | **Sobrevive sem mudança de promessa** | Lei 8.935/94 confirmada verbatim por F1 e F4 ✅ |
| `responsabilidade-e-pad` | ⚠️ **Divide-se em duas** | São regimes distintos: a responsabilidade **civil** é função da **data do ato em três faixas** (objetiva até 21/06/2015 · objetiva pela Lei 13.137/2015 entre 22/06/2015 e 10/05/2016 · subjetiva a partir de 11/05/2016) e tem **dois** termos iniciais de prescrição; o **PAD** não tem rito federal nem prazo prescricional federal — o rito é das Normas de Serviço da CGJ estadual e o prazo é do estatuto de servidores do estado (STJ RMS 72.379). Misturar as duas esconde as três perguntas de abertura da defesa — F4 rev. 2 §§1.2, 1.3, 3.2, 3.3, 10.1 ✅ |
| `emolumentos-nunca-hardcoded` | **Sobrevive, com três correções de conteúdo** | (i) **percentual sobre o valor do negócio é VEDADO** (Lei 10.169/2000, art. 3º II) — a meta o listava como forma possível; (ii) **no DF a base é lei FEDERAL** (Lei 14.756/2023), não estadual; (iii) vale a **tabela do dia do ato** (art. 6º), e o RJ teve duas vigências em 2026 — F5 §§1.1, 1.2, 7 ✅ |
| `codigo-nacional-de-normas-vigente` | **Sobrevive e vira o artefato central — mas muda de forma** | A meta previa "versão consolidada + data de corte". F1 §7 mostra que precisa de **quatro campos que uma skill de gate lê e compara**: data de corte · número do último provimento alterador (hoje **253**) · último id varrido na base do CNJ (hoje **6998**) · lista de suspensos ativos com data-limite. E o artefato base existe e está identificado: o **PDF compilado oficial de 369 páginas**, consolidado até o Prov. 253/2026 — F2 §12.3 ✅ |
| **NOVO — `qualificacao-notarial-transversal`** | ⭐ **Entra** | F2 §12.2: capacidade, legitimidade, licitude e forma (CC 104, 215, 1.647; CNN 111, 145) se repetem nos cinco atos. "Uma skill de qualificação bem feita é reusada cinco vezes; cinco skills de ato com qualificação embutida divergem entre si em três meses" ✅ |
| **NOVO — `pld-ft-e-comunicacao-a-uif`** | ⭐ **Entra** | CNN arts. 145-181 (Prov. 161/2024): cadastro obrigatório com PEP e lista da Lei 13.810/2019, guarda própria de **5 anos** (art. 173), e a trava de mão dupla do art. 179 — recusar por falta de dado só-PLD é infração, **mas** lavrar não dispensa a comunicação à UIF. É fonte autônoma de PAD — F2 §8, F4 §5.3 ✅ |
| **NOVO — `conformidade-de-ia-na-serventia`** | ⭐⭐ **PROMOVIDA a camada de primeira classe (P-1)** | Deixa de ser uma skill da Camada 0 e vira **camada própria** — ver §2.2-bis. Decisão cravada do Doc: é o **diferencial central** do v0.1 |

### 2.2-bis ⭐ Camada C — Conformidade Regulatória de IA na Serventia (P-1, camada de primeira classe)

**Por que é camada e não skill.** As outras camadas do plugin respondem "como o titular pratica o
ato". Esta responde a uma pergunta diferente, que nenhuma outra cobre: **"o titular pode usar esta
ferramenta, e como ele prova isso à Corregedoria?"** Ela tem interlocutor próprio (a CGJ), prazo
próprio (comunicação **anual**; 90 dias de adequação para quem já usa IA), sanção própria (chega a
**falta grave do art. 31 da Lei 8.935/94**) e entregáveis que não se parecem com nenhum outro do
produto — são documentos de governança, não minutas de ato. Tratá-la como apêndice da Camada 0 a
faria herdar o vocabulário errado.

**Os seis artefatos, cada um com o dispositivo que o exige** (✅ Prov. TJMT/CGJ n. 1/2026, capturado
verbatim em `pesquisa/capturas/mercado-provimento-tjmt-1-2026-ia-serventias.md` — F5 §5):

| # | Artefato | Dispositivo | O que é |
|---|---|---|---|
| C-1 | **Análise prévia de risco** da solução de IA | art. 7º, I | Antes de contratar. Classifica o uso contra o Anexo I (o que é ✔ e o que é ✘) |
| C-2 | **Avaliação de impacto no tratamento de dados** | art. 7º, II | Peça de LGPD específica da serventia, com verificação de conformidade e relatório técnico |
| C-3 | **Checklist das 5 cláusulas contratuais mínimas** | art. 8º | Não-treinamento · não-retenção/não-compartilhamento/não-armazenamento de inputs e outputs · compliance LGPD · mecanismos de auditoria · privacy by design e by default |
| C-4 | **Ficha de comunicação anual à Corregedoria** | arts. 6º, V e 12 | Ferramentas usadas, finalidades, incidentes e mitigação. É **anual e obrigatória** |
| C-5 | **Política de registro interno de usos, para auditoria** | art. 6º, VI | A Corregedoria pode pedir relatórios e **logs** a qualquer tempo (art. 13) |
| C-6 | **Roteiro da capacitação obrigatória** | art. 11, V | Cinco conteúdos: fundamentos e limitações da IA · **riscos de vieses, erros e alucinações** · LGPD · casos práticos · ética e supervisão humana. **Renovação a cada 24 meses** |

**Mais dois gates que a camada precisa carregar:** serventia **vaga (interino)** depende de
**autorização prévia da CGJ**, com plano de governança e "valor compatível com o mercado" (art. 9º);
e quem **já usa IA** tinha **90 dias** para adequar, capacitar e comunicar (art. 17).

⚠️ **A fragilidade que a camada tem de declarar em voz alta, e que a própria F5 apontou:** **só MT
regulou até agora.** O produto diz *"em MT já é norma; nas demais UFs é o padrão que está se
formando"* — nunca vende como nacional. Vender norma estadual como se fosse federal é exatamente o
erro que a família já pegou em trânsito e criminal (T-131 · F5 §5.3.5 🟡). E a própria norma
mato-grossense carrega uma trava: ela **se fundamenta no Prov. CNJ 74/2018, revogado 28 dias depois**
pelo Prov. CNJ 213/2026 (T-130 ✅).

**O que a camada NÃO promete:** ela não certifica conformidade nem substitui parecer. Ela **organiza
os documentos que a norma exige** e diz qual dispositivo cobra cada um — o que é exatamente o que o
art. 5º autoriza (organização, sumarização, minuta preliminar sob revisão humana) e o que o art. 4º,
III proíbe que se ultrapasse.

### 2.3 Camada 1 — Atos de balcão (era "Tabelionato de Notas")

| Item | Veredito | Motivo (frente) |
|---|---|---|
| `escritura-publica` | **Sobrevive, com corpus muito maior** | A meta não conhecia **Lei 7.433/85** nem o **Decreto 93.240/86** — que trazem o **rol FECHADO** de documentos, o prazo de 30 dias da certidão do RI e a dispensa das fiscais pelo adquirente. Somam-se a Lei 13.097/2015 (concentração), o **CNN 165-A** (meios de pagamento, obrigação de 2024 que ninguém automatizou) e a camada rural (CCIR sob pena de nulidade, ITR de 5 exercícios) — F2 §3 ✅ |
| `ata-notarial` | ⚠️ **Sobrevive, mas muda de promessa e se divide** | **Não existe norma nacional sobre a ata de constatação** — só CPC 384 + Lei 8.935/94 art. 7º, III; o resto é código estadual (F2 §4.0). E as **atas-instrumento** (usucapião, adjudicação, condição negocial, arrematação) têm regras próprias e **contraditórias entre si** — competência, admissibilidade da declaração do requerente e cláusula de eficácia mudam de uma para a outra (F3 §4.4) ✅ |
| `procuracao-e-testamento` | ⚠️ **Divide-se em duas** | Corpus, precedentes e obrigações periódicas distintos. Procuração: CEP/CENSEC + REsp 1.575.048/SP + o PCA que derrubou o "prazo de validade". Testamento: **remessa quinzenal ao RCTO inclusive negativa** + AR 6.052/SP + regras próprias do cego e de quem não assina — F2 §§5, 6 ✅ |
| `inventario-divorcio-extrajudicial` | ⚠️ **Divide-se em duas e cresce muito** | A Res. CNJ 571/2024 é **maior do que a meta descreveu**: além de incapaz/testamento/alienação pelo inventariante, criou **divórcio com filho menor ou incapaz** (art. 34 §2º), a escritura de **declaração de separação de fato** e a de **restabelecimento da comunhão plena de vida** (arts. 52-A a 52-E — figuras que não existiam), a **certidão por quesitos** (art. 3º § único), e **revogou** os arts. 45 e 47 — F3 §§2.2, 11.5 ✅ |
| `usucapiao-extrajudicial` | **Sobrevive, renomeado** → `ata-de-usucapiao-fase-notarial` | A fase notarial é **um ato**: a ata do inciso I. Todo o resto é do registrador. Competência **vinculada** ao município do imóvel (CNN 402) — F3 §3 ✅ |
| `adjudicacao-compulsoria-extrajudicial` | **Sobrevive, renomeado** → `ata-de-adjudicacao-compulsoria` | Idem, com a correção de fronteira: **a notificação do inadimplente é do OFICIAL DO RI**, não do tabelião (216-B §1º, II) — a meta atribuía o ato ao lado errado — F3 §4.2 ✅ |
| `mediacao-conciliacao-arbitragem-notarial` | ⚠️ **Divide-se em duas** | São regimes distintos: mediação/conciliação são **regulamentadas** (CNN 18-57) e **condicionadas a autorização prévia da CGJ/Nupemec** + listagem pública + curso a cada 2 anos; a **arbitragem não tem rito nenhum** — zero ocorrência de `árbitro/arbitragem/arbitral` no CNN inteiro. Não cabem numa skill só — F3 §§5.2, 5.3, 11.9 ✅ |
| **NOVO — `ata-de-arrematacao-hipotecaria`** | ⭐⭐ **Entra, e é v0.1** | Lei 14.711/2023, art. 9º, §11. A meta a colocou na Camada 2 (RI). É ato do **tabelião de notas**, com **terceira redação de competência** ("circunscrição delegada que abranja o local do imóvel"), conteúdo mínimo **na lei**, efeito **translativo** e **zero regulamentação do CNJ** — o perfil de ato em que o delegatário mais se expõe — F3 §7 ✅ |
| **NOVO — `cessao-de-precatorio-e-as-duas-comunicacoes`** | ⭐ **Entra** | Art. 6º-A da Lei 8.935/94: comunicação da negociação **imediata** + da cessão em **3 dias úteis**, e a **janela de 15 dias corridos** que torna ineficaz a cessão a não identificado. Nenhuma ferramenta de gestão controla esse relógio — F3 §6 ✅ |
| **NOVO — `conta-notarial-vinculada`** | ⭐ **Entra** | Prov. CNJ 197/2025, ancorado no **CNN art. 444-G**. Traz o **único rol de recusa OBRIGATÓRIA** de toda a pesquisa ("o tabelião **deverá** recusar", art. 7º, I a IV) e é o ato de 2025 com maior potencial comercial da vertical. A meta não o conhecia — F3 §§1.1, 9, F2 §4 ✅ |
| **NOVO — `ato-notarial-eletronico-e-competencia`** | ⭐⭐ **Entra** | F2 §7: requisitos do CNN 286 (com o **roteiro obrigatório de 5 itens** da videoconferência), o **algoritmo de competência de 4 passos** (arts. 289, 302-304), as **duas nulidades expressas** (318 e 319 §1º) e a MNE. É determinístico e auditável — exatamente o que um plugin resolve melhor que um manual ✅ |
| **NOVO — `aev-aedo-autocuratela-e-cenad`** | **Entra (menor)** | Módulos criados/alterados entre 2024 e 2026 que a meta não lista: **AEDO** (CNN 444-A a 444-F, Prov. 164/2024), **AEV** (Prov. 103/2020, vivo por remissão no art. 444), **autocuratela e diretivas de curatela** (Prov. 206/2025 + 215/2026, CNN 110-A/110-B), **CENAD** e **e-Not Assina** — F1 §§2, 4.1; F2 §10.6 ✅ |

### 2.4 Camada 2 — Registro de Imóveis

> **Recorte fechado (P-3):** o v0.1 é **Tabelionato de Notas isolado**. O Registro de Imóveis vira
> **plugin-irmão ou v0.2** — o mesmo padrão que a família já validou no cível (nasceu núcleo, cresceu
> depois). O que sobra desta camada no v0.1 é **contexto para orientar**, não skill que executa ato
> alheio: o tabelião tem **dever expresso de orientar** sobre a inviabilidade da via extrajudicial
> (CNN art. 440-G §1º ✅ F3), e não pode orientar sobre o que desconhece.

| Item | Veredito | Motivo (frente) |
|---|---|---|
| `qualificacao-registral-e-duvida` | 🔴 **Não pode ser vendida com esse nome nem com essa promessa** | "Qualificação registral" é **vedação nominal** do art. 4º, II do Prov. TJMT 1/2026 — IA não pode substituir a análise jurídica humana quanto a interpretação normativa, qualificação registral ou enquadramento legal. O que a norma permite (art. 5º, II) é **checklist de exigências + minuta preliminar de nota devolutiva, sob revisão humana**: o titular qualifica, o plugin organiza — F5 §5.3.1 ✅ |
| `usucapiao-extrajudicial-ri` · `adjudicacao-compulsoria-ri` | **Saem da v0.1 como skills de execução — viram contexto** | Se o escopo for Notas isolado, o tabelião ainda precisa **conhecer** a fase registral, porque tem **dever expresso de orientar** sobre a inviabilidade da via extrajudicial (CNN 440-G §1º). Vira material de contexto, não skill que executa ato alheio — F3 §§3.4, 4.3 ✅ |
| `execucao-extrajudicial-hipoteca` | ⚠️ **Muda de camada** | A ponta notarial (a ata de arrematação) **sobe para a Camada 1** como skill própria; a ponta registral (intimação, averbação, registro da ata) fica como contexto — F3 §7 ✅ |
| `serp-e-registro-eletronico` | **Sai da v0.1** | É infraestrutura do registrador. Sem impacto no ato do tabelião de notas — F3 §8 ✅ |

### 2.5 Camadas 3 e 4 — Protesto, RCPN, RTD/RCPJ

**Saem da v0.1**, e o dado sustenta o corte: 3.846 serventias de Protesto e 3.810 de RTD/RCPJ contra
**8.228 de Notas** ✅ F5 §2.1. Duas ressalvas que precisam ficar registradas, porque não são camada
mas são trava:

- **Protesto é fronteira expressa na lei**, não escolha de escopo: o art. 7º-A, I da Lei 8.935/94
  ressalva *"respeitada a competência própria dos tabeliães de protesto"* na certificação de
  implemento/frustração de condição. A certificação de inadimplemento **não é terra livre** ✅ F2 §4.
- **RCPN entra pela porta da responsabilidade, não pela do ato**: o art. 39, **VI** da Lei 8.935/94
  torna o descumprimento comprovado da gratuidade da Lei 9.534/97 hipótese **autônoma de extinção da
  delegação** — e o ofício único do interior acumula Notas + RCPN na mesma porta ✅ F4 §4.

### 2.6 Camada 5 — Transversais

| Item | Veredito | Motivo (frente) |
|---|---|---|
| `varredura-provimento-vigente-pre-lavratura` | **Sobrevive como gate central — com quatro checagens e redação reescrita** | As quatro: (a) situação do provimento (vigente/alterado/**suspenso**); (b) se o dispositivo está superado no consolidado; (c) a **norma da CGJ do estado**, porque precatório, arbitragem e ata de arrematação não têm rito nacional; (d) **o tipo do provimento** (alterador × autônomo × Resolução do Plenário) — F3 §13.4 ✅. E a reescrita: se o gate **decide** se o ato pode ser lavrado, cai no art. 4º, III do Prov. TJMT ("tomada de decisão jurídica, inclusive como instrumento de apoio, sugestão ou influência, ainda que sob revisão humana"); se **exibe a norma vigente com fonte e data** e deixa a decisão ao titular, é art. 5º, I e VII. A diferença é de redação da skill — F5 §5.3.2 ✅ |
| `defesa-tecnica-pad` | **Sobrevive, com as três perguntas de abertura definidas** | (1) qual a data do fato (objetiva × subjetiva); (2) qual a data da portaria de instauração e o que diz o estatuto de servidores **do seu estado** (prescrição — a defesa que mata o processo antes do mérito); (3) o ato já foi anulado em juízo (redefine o triênio civil). E precisa cobrir a **suspensão preventiva** (art. 36: metade da renda travada por até 120 dias), que é o momento de maior disposição a pagar — F4 §§3.3, 3.4, 10 ✅ |
| **NOVO — `nota-fundamentada-de-recusa-e-encaminhamento`** | ⭐⭐ **Entra — três frentes convergem nela** | O corpo normativo exige recusa **fundamentada por escrito** em 4 hipóteses, **encaminhamento ao MP ou ao juízo** em 5, e **consignação no ato** em outras 6 (F3 §9). E **não existe nota devolutiva federal para o tabelião de notas** — ele simplesmente não lavra (F2 §8, F4 §5.4). O termo de recusa não é exigido por norma: é **prova constituída** de que o titular qualificou e decidiu, e é o que responde à representação de "o cartório se recusou sem motivo" (art. 37: qualquer interessado representa) ✅ |
| **NOVO — `calendario-de-obrigacoes-periodicas`** | ⭐ **Entra** | Duas obrigações quinzenais **auditáveis que nenhuma ferramenta encontrada cobre**: remessa ao **RCTO** e à **CESDI** nos dias 5 e 20, **inclusive negativa** (CNN 267 e 270), e a sincronização do **CCN/Índice Único** (CNN 311). Somam-se: comunicação **semestral** de eliminação de documentos (Prov. 50/2015, art. 3º), comunicação **anual** de IA à Corregedoria (Prov. TJMT 1/2026, arts. 6º V e 12), **correição anual** (CNN 105) e incidente de dados em **48 horas úteis** (CNN 91). É calendário, não redação — e é o que aparece em correição — F2 §12.4, F4 §5.3 ✅ |
| **NOVO — `guarda-descarte-e-temporalidade`** | ⭐ **Entra** | Prov. CNJ 50/2015 (adoção tornada **obrigatória** pelo CNN art. 196) com a alteração do **Prov. CN 185, de 26.11.2024**, que rebaixou de Permanente para **5 anos** a guarda de depósito e reconhecimento de firma por autenticidade — condicionado à digitalização com valor legal. E a regra que decorre: **o prazo de guarda é o prazo em que você ainda tem defesa** — o CNJ ancorou a guarda dos documentos que instruíram escritura e procuração no **art. 205 do CC (10 anos)**, não no triênio do art. 22 — F4 §5.2 ✅ |

---

## 3. Consolidado de travas anti-alucinação

As travas das 5 frentes, mescladas, deduplicadas e agrupadas por bloco temático. **Esta lista é o
conteúdo do futuro `context/travas-defasagem.md`.** Cada linha: enunciado · dispositivo/fonte ·
selo · frente de origem. Onde duas frentes trouxeram a mesma trava, a origem aparece composta.

### Bloco A — Vigência e endereçamento normativo (o eixo estrutural desta vertical)

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-01 | O CNN é o **Provimento n. 149, de 30.8.2023**. 4.9.2023 é a **publicação** (DJe/CNJ 207/2023, p. 7-242). Citar o ato pela data do ato, e as duas para não parecer errado | `atos.cnj.jus.br/atos/detalhar/5243` | ✅ | F1, F2 |
| T-02 | Antes de citar qualquer provimento por número, resolver o **estado em três valores**: ABSORVIDO (revogado) · VIVO POR REMISSÃO · SUSPENSO. Citar o número sem o estado é o erro estrutural da vertical | ficha oficial de cada ato no CNJ | ✅ | F1 |
| T-03 | E resolver também o **tipo**: **ALTERADOR** (cite o artigo do CNN, creditando a origem) × **AUTÔNOMO** (cite o provimento **e** o artigo do CNN que remete a ele) × **Resolução do Plenário** (terceiro endereço, **fora** do Código) | Ementa do Prov. 150/2023 + Exposição de Motivos do CNN | ✅ | F3 |
| T-04 | **Nem tudo foi absorvido.** Continuam **vivos por remissão**: 56/2016 (RCTO), 103/2020 (AEV), 62/2017 (apostila, anexos), 50/2015 (temporalidade), 197/2025 (conta notarial), 213/2026 (TI). Tratá-los como "remissão histórica" faz o plugin ignorar norma aplicável | fichas oficiais + arts. 441 II, 444, 444-G do CNN | ✅ | F1, F3 |
| T-05 | **Resoluções do Plenário nunca entraram no CNN** (35/2007, 571/2024, 547/2024, 617/2025). A própria Exposição de Motivos diz que resoluções não foram incorporadas, por serem competência do Plenário | Exposição de Motivos do CNN | ✅ | F1, F3 |
| T-06 | **A Exposição de Motivos do CNN é fonte envelhecida** que parece autoritativa: lista como "conservados" o Prov. 74/2018 e o 39/2014, **ambos revogados depois**. Ela é o retrato de agosto de 2023 | `capturas/cnn-00-metadados-e-alteracoes.md` | ✅ | F1 |
| T-07 | **Suspensos hoje: 172/2024, 175/2024 e 247/2026.** Suspenso **não** é revogado — a ficha do CNJ mostra "Suspenso", e confundir os dois estados é erro real | `detalhar/5614`, `/5666`, `/6956` | ✅ (data e prazo do 247: 🟡) | F1 |
| T-08 | **O art. 440-AO virou de lado em 24-28/07/2026:** alienação fiduciária de imóvel por instrumento particular **liberada dentro e fora do SFI/SFH** (redação do Prov. 246, de 28.7.2026), com vedação expressa de recusa (§3º). Um plugin com corte em 2024/2025 mandaria o tabelião exigir escritura que **não é mais reserva dele** | CNN art. 440-AO, red. Prov. 246/2026 | ✅ | F1 |
| T-08b | **E há MS 40.223 pendente no STF** sobre essa mesma questão — a postura honesta é dizer que a regra vigente é a do Prov. 246 **e que o STF pode mudá-la**, nunca vender a questão como fechada | portal do STF | 🟡 | F1 |
| T-09 | **São 57 alterações do CNN**, não "60+", e a mais recente é o **Provimento n. 253, de 18.8.2026** — não o 246 | lista oficial "Alteração" + corpo consolidado | ✅ | F1, F2, F3 |
| T-10 | **O Provimento 244/2026 não altera o CNN.** A alteração de 21.7.2026 é o **242**; o **244 é de 22.7.2026** e trata de passivos funcionais da magistratura | ficha oficial | ✅ | F1 (corroborado por F4 via ANOREG) |
| T-11 | **Os Provimentos 228 e 229 existem, os dois, com data 16.6.2026** (extratos eletrônicos no RI × ecossistema do SERP). Não são erro de digitação um do outro | texto consolidado do CNN | ✅ | F1, F4 |
| T-12 | **O CNJ não usa tachado no texto compilado — ele EMPILHA as versões etiquetadas.** Dentro de um mesmo dispositivo vence a **última redação por data de provimento**; trecho com `(revogado pelo...)` sai; trecho com `(suspenso por força da decisão...)` **não pode ser citado como norma viva**. É armadilha diferente da do Planalto (lá o revogado vem riscado) | HTML do texto compilado, 0 ocorrências de `line-through`/`<strike>`/`<del>` | ✅ | F1 |
| T-13 | **A Parte Geral do CNN tem 6 Livros, não 5** — o Livro VI ("De Outras Regras Comuns às Especialidades", art. 353-A) foi acrescido depois | estrutura do texto compilado | ✅ | F1 |
| T-14 | **O corpus notarial está em 4 endereços**, e "abrir o livro de notas" entrega 5 capítulos residuais: (a) Parte Geral Livros I-III e V-VI; (b) **Parte Geral Livro IV, Cap. VI, arts. 264-319** — o núcleo, e-Notariado/CENSEC; (c) Parte Especial Livro III (atas de usucapião e adjudicação); (d) Parte Especial Livro IV, arts. 441-444-G | contagem de ocorrências no texto compilado | ✅ | F1 |
| T-14b | **Nuance:** o Livro IV da Parte Especial não é *puramente* residual — três dos cinco capítulos são remissões, mas os **arts. 444-A a 444-G são camada nova** (AEDO, 2024; conta notarial vinculada, 2025) | CNN 444-A a 444-G | ✅ | F2 (precisa a leitura de F1) |
| T-15 | **Arbitragem notarial tem ZERO ocorrência no CNN** (`árbitro`/`arbitragem`/`arbitral` no texto inteiro). A base legal existe (art. 7º-A, III); o **rito nacional não** | busca literal no texto integral | ✅ | F1, F3 |
| T-16 | **`precatório` também tem ZERO ocorrência no CNN.** Não há regulamentação nacional da competência do art. 6º-A. O que existe é norma **estadual** (SP, Prov. CSM 2.753/2024) | busca literal + varredura em `cnj.jus.br` | ✅ (a busca) / 🟡 (a ausência absoluta) | F3 |
| T-17 | **O CNN quase não regula o CONTEÚDO do ato notarial.** Escritura, procuração e testamento vivem no **CC/2002**, na **Lei 8.935/94** e nos **códigos de normas estaduais** de cada TJ, que convivem com o CNN e não foram substituídos por ele | CNN + CNFE/TJPR como exemplo verificado | ✅ | F1 |
| T-18 | **A rotina de refresh precisa vigiar provimento AUTÔNOMO que não altera o CNN.** O Prov. 247/2026 (VNS) é a prova: não alterou o Código, criou cobrança por ato e foi suspenso em menos de uma semana. Quem só vigia a ficha do CNN **não veria isso** | `detalhar/6956` | ✅ | F1 |

### Bloco B — Qual lei trouxe qual instituto

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-19 | **O art. 216-B da LRP (adjudicação compulsória extrajudicial) é da Lei 14.382/2022**, não da 14.711/2023 — cada dispositivo traz o rótulo "(Incluído pela Lei nº 14.382, de 2022)" | Lei 6.015/73 compilada | ✅ | F3 (confirma a correção que a meta já fizera ao briefing) |
| T-20 | **O art. 7º-A da Lei 8.935/94 é INTEIRO da Lei 14.711/2023.** Da Lei 14.382/2022 são **só os §§ 1º a 5º do art. 7º**. A meta se contradiz aqui, atribuindo o 7º-A às duas leis em linhas consecutivas | Lei 8.935/94 compilada | ✅ | F3 |
| T-21 | **6º-A = cessão de precatório. 7º-A = condição negocial + mediação/conciliação + arbitragem + conta vinculada.** São competências diferentes, não um bloco | Lei 8.935/94 | ✅ | F3 |
| T-22 | **Regra mnemônica:** 14.382/2022 = **REGISTRO** (a lei do SERP); 14.711/2023 = **GARANTIA** (Marco das Garantias). Se o dispositivo dá **poder novo ao tabelião de notas**, é a **14.711/2023** — única exceção, os §§ 1º-5º do art. 7º | — | ✅ | F3 |
| T-23 | **O § 7º do art. 7º da Lei 8.935/94 foi VETADO** (assim como o § 6º) — e o § 3º do art. 7º-A **remete a ele**. Defeito de remissão no texto vigente; o parâmetro remuneratório que sobra é o do próprio § 3º *in fine* | Planalto, texto compilado | ✅ (o veto) / 🟡 (a consequência) | F3 |
| T-24 | **Os §§ 3º e 4º do art. 39 da Lei 8.935/94, incluídos pela Lei 14.711/2023, foram VETADOS.** Citar "§ 3º do art. 39 incluído pelo Marco das Garantias" é alucinação | Planalto, texto consolidado | ✅ | F4 |

### Bloco C — Competência territorial

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-25 | **A livre escolha do art. 8º NÃO sobrevive no ato eletrônico.** Ali a competência é **exclusiva e ABSOLUTA**, observada a circunscrição da delegação | Lei 8.935/94 arts. 8º e 9º; **CNN art. 289** (verbatim: "é absoluta") | ✅ | F2 |
| T-26 | **A competência do ato eletrônico é um algoritmo de 4 passos, não uma regra única.** Escritura → circunscrição do imóvel **ou** domicílio do adquirente (302); ata → circunscrição do fato **ou** domicílio do requerente (303); procuração → domicílio do outorgante **ou** local do imóvel (303 § único). E o **§2º do art. 302 devolve a escolha dentro da mesma UF** quando imóvel e domicílio do adquirente coincidem no estado | CNN arts. 302-304 | ✅ | F2 |
| T-27 | **Há TRÊS redações diferentes de competência vinculada, e não são intercambiáveis:** usucapião = "município em que estiver localizado o imóvel **ou a maior parte dele**" (CNN 402); adjudicação = **livre escolha do requerente**, salvo se envolver diligência no local (CNN 440-F); arrematação hipotecária = "tabelião com **circunscrição delegada que abranja o local do imóvel**" (Lei 14.711/2023, art. 9º §11) | as três normas | ✅ | F2, F3 |
| T-28 | **A competência do ato notarial HÍBRIDO não está resolvida.** O CNN art. 313 autoriza o ato com uma parte assinando fisicamente e outra a distância, mas não diz se seguem os arts. 302-304 ou o art. 8º. É pergunta que o usuário faz na primeira semana | CNN art. 313 | 🔴 | F2 |

### Bloco D — Qualificação, capacidade e PLD

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-29 | **Exigir testemunha só porque a parte tem deficiência é ILEGAL.** Lei 8.935/94 art. 7º §2º (Lei 14.382/2022) veda expressamente; e o CC art. 228, **II e III foram revogados** pela Lei 13.146/2015, com §2º garantindo o testemunho em igualdade com tecnologia assistiva. **Exceção — a "disposição em contrário":** o testamento do cego (CC 1.867, com dupla leitura). Manual pré-2015 ensina a prática hoje ilegal | Lei 8.935/94 art. 7º §2º; CC 228 e 1.867 | ✅ | F2 |
| T-30 | **Absolutamente incapaz é só o menor de 16 anos** (CC art. 3º, red. Lei 13.146/2015 — incisos I, II e III revogados). O art. 4º traz os relativamente incapazes, incluindo quem "não puder exprimir sua vontade" | CC arts. 3º e 4º | ✅ | F2 |
| T-31 | **A qualificação das partes tem conteúdo obrigatório**, inclusive a **existência de união estável** (CNN art. 111) — e, em ato protocolar com conteúdo econômico, o cadastro do CNN art. 145 (Prov. 161/2024) alcança **representantes e procuradores**, com estado civil e qualificação do cônjuge "em qualquer hipótese", lista de sanções da Lei 13.810/2019 e enquadramento como **PEP** | CNN arts. 111 e 145 | ✅ | F2 |
| T-32 | **Falta de dado de PLD NÃO autoriza recusa — e há um caminho positivo no lugar dela.** A regra de ouro: o tabelião **lavra**, **CONSIGNA a recusa da parte no corpo da escritura** (165-A §3º) e **comunica à UIF** quando for o caso. *"Recusar o ato é que gera infração; consignar é que gera prova."* Ensinar "sem a origem dos recursos, não lavro" é ensinar infração. **Mas a mão inversa também erra:** praticar o ato não dispensa a comunicação quando cabível | **CNN art. 179** (verbatim, Prov. 161/2024) + 165-A §3º + 155-A VIII | ✅ | F2 (apontou) + F4 rev. 2 (**reverificou na fonte** antes de incorporar) |
| T-33 | **A documentação de PLD tem guarda própria de 5 anos**, contados da prática do ato, sem prejuízo de prazos maiores de outras leis | CNN art. 173 (Prov. 161/2024) | ✅ | F4 |

### Bloco E — Escritura pública

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-34 | **O rol de documentos da escritura é FECHADO**, não aberto: *"além dos documentos de identificação das partes, **somente** serão apresentados os documentos expressamente determinados nesta Lei"*. Quem detalha é o Decreto 93.240/86, art. 1º (I a V) — com **validade de 30 dias** para a certidão de ações reais/reipersecutórias e de ônus reais (inciso IV) | **Lei 7.433/85, art. 1º caput** + Decreto 93.240/86 | ✅ | F2 |
| T-35 | **As certidões fiscais municipais podem ser dispensadas pelo adquirente**, que então responde pelos débitos — e o outorgante **declara na escritura, sob pena de responsabilidade civil e penal**, a existência de outras ações reais e ônus | Decreto 93.240/86, art. 1º §§2º e 3º | ✅ | F2 |
| T-36 | **"Feitos ajuizados" saiu da lei.** A redação vigente (Lei 13.097/2015) fala em **certidões fiscais e certidões de propriedade e de ônus reais** — repetir a expressão de 1985 é defasagem de 40 anos | Lei 7.433/85, art. 1º §2º | ✅ | F2 |
| T-37 | **A concentração na matrícula é a Lei 13.097, de 19 de janeiro de 2015** (não 2016), e o **inciso V do art. 54 é de 2024** (Lei 14.825) — posterior ao próprio CNN | Lei 13.097/2015, art. 54 | ✅ | F2 |
| T-38 | **Certidão negativa fiscal é INFORMAÇÃO, não CONDIÇÃO.** O Plenário do CNJ proibiu exigir CND/CPEN como condição para registrar ou averbar compra e venda de imóvel — é cobrança indireta de tributo. **Mas as duas metades andam juntas:** o cartório **pode** solicitar a certidão para informar a situação do vendedor, desde que não impeça o ato | **PCA 0001611-12.2023.2.00.0000**, rel. Cons. Marcello Terto, 10ª Sessão Virtual/2025, notícia oficial 08/09/2025 | ✅ | F2 |
| T-38b | **Não confundir CND/CPEN com CNDT.** O art. 47, I, "b" da Lei 8.212/91 **continua no texto vigente**; o que o CNJ afastou foi a exigência **como condição**. E há discussão paralela sobre débitos trabalhistas que não foi fechada | Lei 8.212/91, art. 47 | 🔴 (a CNDT) | F2 |
| T-39 | **CCIR ausente em imóvel rural = NULIDADE cominada em lei**, não formalidade menor: sem o Certificado de Cadastro não se pode desmembrar, arrendar, hipotecar, vender ou prometer em venda, "sob pena de nulidade"; e nenhuma partilha se homologa sem ele | **Lei 4.947/66, art. 22, §§1º e 2º** | ✅ | F2 |
| T-40 | **ITR dos cinco últimos exercícios** é exigência legal para os atos dos arts. 167 e 168 da LRP, com **responsabilidade solidária** — mas a responsabilidade nominada é do **serventuário do registro de imóveis**, não do tabelião de notas. Para o tabelião é item de qualificação (Decreto 93.240, III "b"). **Não fundir os dois** | Lei 9.393/96, art. 21 e § único | ✅ / 🟡 na extensão ao tabelião | F2 |
| T-41 | **Toda escritura de direito real imobiliário deve indicar, de forma precisa, MEIOS E FORMAS DE PAGAMENTO** — espécie com local e data; transferências com identificação inequívoca das contas; cheques; **ativos virtuais**, dação, permuta; e o meio **de cada parcela**. Terceiro pagador é **qualificado na escritura** (§2º) e a **recusa da parte em informar deve ser mencionada** (§3º) | **CNN art. 165-A** (Prov. 161/2024) | ✅ | F2 |
| T-42 | **O CNN se contradiz duas vezes em torno do 165-A:** (a) **remissão órfã** — o §3º remete literalmente ao "art. 155, VIII", mas o art. 155 foi **revogado pelo mesmo Prov. 161/2024**; o conteúdo vivo (resistência da parte em fornecer informação → sinal de alerta) está no **art. 155-A, VIII**. **Regra: citar o §3º verbatim E apontar a migração — nunca escolher um dos dois em silêncio**, porque citar "155" reproduz remissão a dispositivo revogado e citar "155-A" acerta o conteúdo mas não é o que o §3º literalmente diz; (b) o **art. 109** dispensa a inserção da condição de PEP nos atos protocolares e nas escrituras, colidindo com o 165-A que a **exige**. **Nunca citar o art. 109 sozinho** — seria ensinar o tabelião a omitir o que a norma posterior e especial exige | CNN arts. 109, 155, 155-A, 165-A | ✅ (os textos e a remissão órfã) / 🟡 (a reconciliação do 109 × 165-A) | F2 + F4 rev. 2 (R16 — a regra "citar os dois" é da F4) |
| T-43 | **A estrutura da escritura é lei, com sete incisos** — inclusive o **reconhecimento da identidade e capacidade** de todos os comparecentes (II), a **referência ao cumprimento das exigências legais e fiscais** (V) e a **declaração de leitura na presença de todos** (VI) | CC art. 215, §1º | ✅ | F2 |
| T-44 | **"Separação absoluta" (CC 1.647) não é sinônimo de separação obrigatória (CC 1.641).** A dispensa de outorga conjugal no regime **obrigatório** é controvertida (Súmula 377/STF e sua leitura atual). O plugin marca divergência, não decide | CC arts. 1.641, 1.647-1.649 | 🟡 / 🔴 na súmula | F2 |
| T-45 | **Doação tem três nulidades próprias que o tabelião apura no ato:** adiantamento de herança entre ascendente/descendente e cônjuges (544 → cláusula de colação ou dispensa); **nula** a doação universal sem reserva de subsistência (548); **nula** a parte inoficiosa que excede o disponível (549) — o que obriga a apurar a legítima **no momento da liberalidade** | CC arts. 544, 548, 549 | ✅ | F2 |
| T-46 | **A base dos "30 salários mínimos" do CC art. 108 não está dirimida** (valor do negócio × venal × base do ITBI). Declarar a divergência, não escolher em silêncio | CC art. 108 | 🔴 | F2 |

### Bloco F — Ata notarial

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-47 | **Não existe capítulo geral de ata notarial no CNN.** As ~21-22 ocorrências são todas em contextos específicos. A ata de **constatação** — a mais volumosa e a que mais cresce — tem só três âncoras nacionais: **CPC art. 384**, **Lei 8.935/94 art. 7º, III** (exclusividade) e o art. 22 para a responsabilidade. Todo o resto é **código estadual de normas** | varredura das 369 pp. do compilado | ✅ | F2 |
| T-48 | **Toda ata deveria carregar três cláusulas**, extraídas dos dois únicos modelos nacionais: (i) **alerta de crime de falsidade** ao requerente e às testemunhas; (ii) **cláusula de não-eficácia**; (iii) **não se basear apenas na declaração do requerente** | CNN arts. 402 e 440-G | ✅ (as normas) / 🟡 (a generalização) | F2 |
| T-49 | **Usucapião e adjudicação NÃO seguem a mesma regra — e estão em artigos consecutivos.** Usucapião: competência **vinculada**, **vedado** basear-se só na declaração do requerente (402 §2º), ressalva "não tem valor como confirmação ou estabelecimento de propriedade" (402 §3º), alerta a requerente **e** testemunhas. Adjudicação: **livre escolha** salvo diligência no local (440-F), a declaração do requerente **pode compor a prova** (440-G §5º), ressalva "não tem valor de título de propriedade" **+ "poderá ser aproveitada em processo judicial"** (440-G §2º), e **dever de orientar sobre a inviabilidade** da via extrajudicial (440-G §1º) | CNN 402 × 440-F/440-G | ✅ | F3 |
| T-50 | **A ata de arrematação hipotecária É TÍTULO TRANSLATIVO** — "constituirá título hábil de transmissão da propriedade ao arrematante a ser registrado na matrícula". Copiar nela a cláusula de não-eficácia das outras duas deixa o ato **errado por excesso** e o arrematante não registra | **Lei 14.711/2023, art. 9º, §11** | ✅ | F3 |
| T-51 | **e-Not Provas ≠ ata notarial.** O e-Not Provas é plataforma do CNB dentro do e-Notariado em que **o próprio cliente** faz as capturas e recebe autenticação de prova digital — **self-service, sem diligência do tabelião**. A ata do art. 384 continua sendo ato **do tabelião**, que descreve o que **ele** constatou. Tratar como sinônimos entrega ao titular um produto que **não é dele** e apaga o serviço onde há emolumento e responsabilidade | documentação oficial do CNB (`suporte.notariado.org.br`) | ✅ / 🟡 na distinção jurídica | F2 |
| T-52 | **Exceção rara à regra "nunca hardcodar emolumento":** enquanto não houver lei estadual, **a ata notarial de usucapião é ato de conteúdo econômico**, com base no valor venal do último IPTU/ITR ou, na falta, no valor de mercado aproximado. É regra **supletiva** e cede diante de lei estadual — o plugin diz as duas coisas | **CNN art. 423, I** | ✅ | F2 |

### Bloco G — Procuração pública

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-53 | **Poder genérico não é poder especial.** "Poderes para vender e doar quaisquer bens" **não basta**: exige-se **bem individualizado** e, na doação, **donatário nomeado**. A falta gera **nulidade** (CC 166, IV e V) | **REsp 1.575.048/SP** (4ª T., Marco Buzzi, un., 23/02/2016) + **REsp 503.675/SP** (3ª T., Nancy Andrighi, 03/05/2005); CC arts. 657 e 661 §1º | ✅ | F2 |
| T-54 | **Procuração pública NÃO tem prazo de validade.** Exigir "expedida há no máximo 30 dias" é **ato ilegal** — "não encontra amparo na legislação vigente", salvo hipótese legal ou fundamentação idônea. O dever do art. 150 do CNN é **verificar** a atualidade, e a abstenção só é devida quando o tabelião **tem conhecimento** de revogação | **PCA 0007885-89.2023.2.00.0000**, rel. Cons. Marcello Terto, 8ª Sessão Virtual, notícia oficial 25/06/2025 + CNN art. 150 | ✅ | F2 |
| T-55 | **A CEP responde SE existe, não O QUE diz.** A consulta traz serviço, data, livro e folhas, e apenas se o ato é escritura ou procuração — *"vedado o detalhamento da modalidade de negócio e demais informações relativas ao objeto ou partes"*. Para conferir a **extensão dos poderes** é preciso ir ao notário emitente. O plugin não pode prometer que a central resolve sozinha | CNN art. 273 (red. Prov. 194/2025 e 209/2025) + art. 301 §1º | ✅ | F2 |
| T-56 | **Morte extingue o mandato (CC 682, II) — salvo a procuração em causa própria (CC 685)**, que não se extingue pela morte de qualquer das partes. Aceitar procuração comum de outorgante falecido é lavrar ato ineficaz | CC arts. 682 e 685 | ✅ | F2 |
| T-57 | **Revogação e rerratificação têm comunicação obrigatória ao notário emitente**, com anotações remissivas nas duas escrituras — **independentemente** da informação à CEP. E todo substabelecimento/revogação exige a menção de notário, livro, folhas, protocolo e data do ato anterior | CNN arts. 272 §4º e 307 | ✅ | F2 |
| T-58 | **Substabelecimento particular de mandato público**, quando o ato-fim exige forma pública, é tensão não resolvida (CC 655 × 657). Sem jurisprudência dirimente localizada | CC arts. 655, 657 | 🔴 | F2 |

### Bloco H — Testamento público

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-59 | **Testamento público exige DUAS testemunhas**, a um só tempo, com leitura em voz alta. Cinco testemunhas é o CC/1916 — manual antigo está no Código revogado | CC art. 1.864, II | ✅ | F2 |
| T-60 | **O discernimento se afere NO ATO.** Incapacidade superveniente não invalida; capacidade superveniente não convalida. É a cláusula mais importante da minuta e a principal defesa do titular em anulatória | CC arts. 1.860 e 1.861 | ✅ | F2 |
| T-61 | **Ao cego só se permite o testamento público, com DUPLA leitura** — uma pelo tabelião, outra por testemunha designada pelo testador, com menção circunstanciada. É a "disposição em contrário" que ressalva a T-29 | CC art. 1.867 | ✅ | F2 |
| T-62 | **A remessa quinzenal ao RCTO é obrigatória INCLUSIVE NEGATIVA** — até o dia **5** (2ª quinzena do mês anterior) e até o dia **20** (1ª quinzena do mês corrente), com nome, RG, **CPF**, espécie e data do ato, livro e folhas, arquivando-se o comprovante. O cartório que não lavrou testamento **tem de informar isso mesmo assim** | **CNN art. 267** | ✅ | F2 |
| T-63 | **A consulta ao RCTO é OBRIGATÓRIA antes do inventário/partilha/divórcio extrajudicial** — gate de entrada, não sugestão. O CNN remete nominalmente ao **Provimento 56/2016**, que continua vigente | CNN art. 441, II | ✅ | F2, F3 |
| T-64 | ⭐ **O precedente que "flexibiliza" o testamento NOMEIA o notário.** A tese publicada diz que a mácula *"decorre de conduta atribuível **exclusivamente ao notário** responsável pela prática do ato"* — um enunciado que declara **autoria exclusiva** entrega, de graça, o **nexo causal** de uma futura ação de reparação. O ato é salvo **em nome de terceiros de boa-fé**, não do tabelião. **Nunca apresentar como precedente favorável ao titular — é mapa de risco** | **AR 6.052/SP**, 2ª Seção do STJ, rel. Min. Marco Aurélio Bellizze, un., 08/02/2023, DJe 14/02/2023, Informativo 775, verbatim em `capturas/resp-stj-ar-6052-testamento-culpa-do-notario.md` | ✅ | F2 (apontou) + F4 rev. 2 (**verificou independentemente**, R18) |
| T-64b | **E o vício era procedimental e evitável:** assinaturas colhidas **em momentos diversos**, quebrando a **unicidade** do ato testamentário, mais leitura incerta. Isso é item de **checklist** — presença simultânea, leitura em voz alta, ordem e horário das assinaturas, tudo consignado. Some-se: **só o substituto não pode lavrar testamento** (art. 20 §4º), ou seja, é justamente o ato **indelegável do titular** que produz o precedente que o nomeia | CC art. 1.864, II + Lei 8.935/94, art. 20 §4º | ✅ | F4 rev. 2 |
| T-64c | **O testamento é o caso extremo da T-97 (*actio nata*), e prova que ela não é exceção de nicho.** Testamento tem guarda **Permanente** (Tabela de Temporalidade, cód. 3-5-1-2) e sua eficácia se opera com o **falecimento do testador** — que pode vir décadas depois da lavratura. Se o triênio contasse literalmente da lavratura, a pretensão contra o notário **nasceria prescrita em praticamente todo testamento** | AR 6.052/SP + Prov. CNJ 50/2015 + art. 22 § único | ✅ | F4 rev. 2 |
| T-65 | **A flexibilização tem limite** — e-mail sem assinatura não vale como testamento particular (REsp 2.115.909/SP, 3ª T., 16/06/2026). Número e data vêm de fonte secundária idônea; **acórdão não lido** | Migalhas / CNB-SP | 🟡 | F2 |

### Bloco I — Ato notarial eletrônico

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-66 | **A videoconferência notarial tem roteiro obrigatório de CINCO itens** que precisam ser falados e gravados: identificação, capacidade e livre manifestação **atestadas pelo tabelião**; consentimento e concordância; **objeto e preço**; data e horário; e livro, página e tabelionato em que será lavrado | **CNN art. 286, § único** | ✅ | F2, F4 |
| T-67 | **Duas nulidades expressas no eletrônico:** ato lavrado **sem o selo** exigido pelas normas estaduais é **nulo** (art. 319 §1º, red. Prov. 202/2025); e é **vedada** a colheita de assinatura eletrônica a distância **fora do e-Notariado** (art. 318) — plataforma privada de terceiro ou gov.br não servem | CNN arts. 318 e 319 | ✅ | F2 |
| T-68 | **O ato eletrônico não é opcional para a serventia:** *"Todos os tabeliães de notas deverão prestar o serviço"* | CNN art. 284, § único (Prov. 181/2024) | ✅ | F2 |
| T-69 | **A MNE tem 24 dígitos** em seis campos, com 2 verificadores gerados pelo **Módulo 97 Base 10, ISO 7064:2003**; o número **integra** o ato, e traslados e certidões conterão **obrigatoriamente** a expressão de consulta de validade | CNN art. 295 e §§2º e 3º | ✅ | F2 |
| T-70 | **A dispensa do selo do art. 319 alcança só quatro módulos** — CENAD, e-Not Assina, **AEV** e **AEDO** (art. 319 §2º; Prov. 178/2024). Não é dispensa geral | CNN art. 319 §2º | ✅ | F1, F2 |

### Bloco J — Desjudicialização

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-71 | **Tensão CPC × Resolução, e o produto tem de dizê-la em voz alta.** O **CPC art. 610, caput** manda ao inventário **judicial** havendo testamento ou incapaz; o **art. 733, caput** condiciona o divórcio extrajudicial a **não haver** nascituro ou filhos incapazes. Quem abriu essas hipóteses foi uma **Resolução do CNJ**, não uma lei. O tabelião **segue a Resolução** (é a norma correicional dele), mas o ato pode ser atacado por terceiro invocando a letra do CPC — a blindagem é documentar integralmente os requisitos cumulativos no ato | CPC 610 e 733 × Res. 35/2007, arts. 12-A, 12-B e 34 §2º | ✅ (os textos) / 🔴 (o desfecho: nenhuma ADI ou precedente vinculante encontrado) | F3 |
| T-72 | **A Res. CNJ 571/2024 é maior do que a meta descreveu.** Além de incapaz (12-A), testamento (12-B) e alienação pelo inventariante (11-A), ela permitiu **divórcio com filho menor/incapaz** mediante prévia resolução **judicial** de guarda, visitação e alimentos consignada na escritura (34 §2º); **criou** a escritura de **declaração de separação de fato** e a de **restabelecimento da comunhão plena de vida** (52-A a 52-E); criou a **certidão/traslado por quesitos** (3º § único); e **revogou** os arts. 45 e 47 | Res. CNJ 571/2024 | ✅ | F3 |
| T-73 | **Quatro figuras que se confundem, e é o erro mais provável da camada:** separação **consensual** (extinta como ato novo — art. 47 revogado) · separação **de fato** (nova, 52-A) · restabelecimento da **sociedade conjugal** (velho, arts. 48-51, inclusive de separação judicial) · restabelecimento da **comunhão plena de vida** (novo, 52-C) | Res. 35/2007, Seções IV e V | ✅ | F3 |
| T-74 | **No inventário com incapaz, o MP é gate de EFICÁCIA, não de lavratura.** A escritura existe, mas **não produz efeito** sem manifestação favorável do MP — e **cabe ao tabelião encaminhar** o expediente. Impugnação do MP ou de terceiro remete ao juízo | Res. 35/2007, art. 12-A §§3º e 4º | ✅ | F3 |
| T-75 | **Vedações duras do inventário/divórcio extrajudicial:** recolhimento dos tributos **antecede** a lavratura (art. 15); **vedado** inventário de **bens no exterior** (art. 29); **vedado indicar advogado** às partes — recomenda-se Defensoria ou Seccional (art. 9º); advogado ou defensor **obrigatório para todas as partes**, com qualificação e assinatura no ato (CPC 610 §2º e 733 §2º); testamento com **reconhecimento de filho ou outra declaração irrevogável** torna o inventário **obrigatoriamente judicial** (12-B §1º) | Res. 35/2007 + CPC | ✅ | F3 |
| T-76 | **Na adjudicação compulsória, a notificação do inadimplente é do OFICIAL DO RI** (que pode delegar ao RTD), não do tabelião de notas. A meta atribuía o ato ao lado errado | LRP art. 216-B, §1º, II | ✅ | F3 |
| T-77 | **A qualificação negativa da adjudicação alcança expressamente o tabelião e não decai:** *"A qualificação **notarial** ou registral será negativa sempre que se verificar, **em qualquer tempo do processo**, ilicitude, fraude à lei ou simulação"* | CNN art. 440-I | ✅ | F3 |
| T-78 | **Mediação e conciliação notariais têm GATE ADMINISTRATIVO prévio.** O plugin não pode sugerir que "o tabelião passe a mediar": exige **autorização** processada por Nupemec/CGJ, inscrição em **listagem pública** da corregedoria, e **curso de aperfeiçoamento comprovado a cada 2 anos**; no máximo **5 escreventes habilitados** sob supervisão do delegatário | CNN arts. 19-23 | ✅ | F3 |
| T-79 | **É VEDADO à serventia estabelecer cláusula compromissória** de conciliação ou mediação extrajudicial nos documentos que expede | CNN art. 56 | ✅ | F3 |
| T-80 | **O termo de acordo é documento público com força de TÍTULO EXECUTIVO EXTRAJUDICIAL**; e direito **indisponível mas transigível** exige **homologação em juízo**, com o cartório encaminhando os autos e entregando o termo homologado às partes | CNN arts. 28 §§1º-2º e 38 § único; CPC 784, IV | ✅ | F3 |
| T-81 | **Conflito real de parâmetro remuneratório da mediação:** o **CNN art. 52** manda usar a tabela do **menor valor de escritura SEM valor econômico**; a **Lei 8.935/94, art. 7º-A §3º** manda usar a tabela de escritura **COM** valor econômico. Regulamentar-supletivo × legal-supletivo, sem solução na fonte | CNN 52 × Lei 8.935/94 7º-A §3º | 🟡 (conflito declarado, não resolvido) | F3 |
| T-82 | **Cessão de precatório: duas comunicações e um relógio.** Negociação → comunicação **imediata**; cessão → **3 dias úteis** da assinatura. E a **janela de 15 dias corridos** do recebimento pelo juízo, dentro da qual a escritura precisa ser lavrada para que a cessão a pessoa não identificada seja **ineficaz**. Passou o prazo, a blindagem cai | Lei 8.935/94, art. 6º-A e §1º | ✅ | F3 |
| T-83 | **A conta notarial vinculada traz o único rol de recusa OBRIGATÓRIA da vertical** — *"o tabelião **deverá** recusar"*: condições não objetivamente verificáveis, direitos indisponíveis ou atípicos, PJ em situação fiscal irregular ou sob investigação judicial, indícios de fraude ou ilicitude. E, havendo **divergência** entre as partes sobre o implemento, o tabelião **documenta em ata, suspende a movimentação e NÃO decide** sobre eficácia ou rescisão | Prov. CNJ 197/2025, arts. 5º §4º, 7º e 9º | ✅ | F3 |
| T-84 | **ITCMD: nunca alíquota.** A LC 227/2026 (vigente 13/01/2026) fixa **normas gerais**; alíquota é **lei estadual** sob teto do Senado, progressiva **por faixa**. E a linha entre renúncia **abdicativa** (não incide) e **translativa** (incide como doação) é qualificação de altíssimo risco: só não incide se feita **sem ressalva ou condição, em benefício do monte**, e se o renunciante **não praticou ato de aceitação** | LC 227/2026, arts. 148, 150, 156-158 | ✅ | F3 |
| T-85 | **O tabelião não lança nem arrecada ITCMD — mas fiscaliza a multa.** A escritura pode ser lavrada a qualquer tempo, "cabendo ao tabelião fiscalizar o recolhimento de eventual multa, conforme legislação tributária estadual". E na partilha desigual ou na transmissão entre cônjuges, comprova-se o tributo **sobre a fração transferida** | Res. 35/2007, arts. 31 e 38 | ✅ | F3 |

### Bloco K — Emolumentos

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-86 | **É VEDADO fixar emolumento em percentual sobre o valor do negócio jurídico.** A estrutura legal é **faixa com mínimo e máximo** para ato com conteúdo financeiro (2º III b) ou **valor por espécie de ato** para ato sem conteúdo financeiro (2º III a). **A meta listava "percentual sobre o negócio" como forma possível — ensinaria prática vedada ao próprio delegatário** | **Lei 10.169/2000, art. 3º, II** | ✅ | F5 |
| T-87 | **Não são "27 tabelas estaduais".** São **26 leis estaduais + 1 lei FEDERAL** — no DF a base é a **Lei 14.756/2023**, com tabelas no anexo da própria lei e atualização anual pelo IPCA. E **cada UF tem várias tabelas** (SP tem cinco). "Confira a tabela do seu estado" quebra no DF | Lei 14.756/2023; `extrajudicial.tjsp.jus.br` | ✅ | F5 |
| T-88 | **No DF, ato fora da tabela é GRATUITO**, "e não se permite interpretação que faça incidir sobre eles qualquer cobrança, mesmo por analogia, paridade ou extensão" — regra dura que não existe em toda UF | Lei 14.756/2023, art. 2º §1º | ✅ | F5 |
| T-89 | **Vale a tabela vigente ao tempo da prática do ato**, não a de hoje; e o reajuste observa a **anterioridade**, publicado até o último dia do ano. O RJ teve **duas vigências dentro de 2026** (01/01-08/03 e a partir de 09/03) | Lei 10.169/2000, arts. 5º e 6º; Portaria CGJ/RJ | ✅ | F5 |
| T-90 | **O único percentual federal que existe é um TETO, não uma forma de fixação:** crédito rural, **0,3%** do crédito concedido (ou o valor da tabela estadual, o menor deles); cancelamento, **0,1%** | Lei 10.169/2000, art. 2º §2º (Lei 13.986/2020) | ✅ | F5 |
| T-91 | **Vedado cobrar retificação de ato refeito ou renovado por erro do próprio serviço** (art. 3º IV) e **vedado cobrar quantia fora da tabela** (art. 3º III). Cobrança indevida ou excessiva, ainda que sob alegação de urgência, é **infração disciplinar** com o PAD do art. 32 na ponta | Lei 10.169/2000, arts. 3º e 7º; Lei 8.935/94, art. 31, III | ✅ | F5 |
| T-92 | **A base de cálculo o plugin PODE determinar; o valor, não.** Regra dominante na amostra: prevalece **o MAIOR entre** valor declarado pelas partes, valor tributário/venal do imóvel e base de cálculo do ITBI; havendo avaliação judicial ou fiscal exigida por lei, é ela | Lei SP 11.331/2002, art. 7º; RJ, notas integrantes; Lei 10.169/2000, art. 2º §1º | ✅ | F5 |
| T-93 | **Afixar a tabela em local visível, observá-la e dar recibo são DEVERES LEGAIS do titular** — "consultar a tabela" não é conselho | Lei 10.169/2000, art. 4º; Lei 8.935/94, art. 30, VII a IX | ✅ | F2, F5 |
| T-94 | **No inventário/divórcio a gratuidade se obtém por SIMPLES DECLARAÇÃO**, mesmo com advogado constituído — e é **vedada** a fixação de emolumentos em percentual sobre o valor do negócio também aqui | Res. 35/2007, arts. 5º, 6º e 7º | ✅ | F3 |
| T-95 | **Os atos preparatórios da ata de usucapião são AUTÔNOMOS para efeito de cobrança** (diligências, reconhecimentos, escrituras declaratórias, notificações, certidões, buscas, editais), com despesas **adiantadas pelo requerente**; e a ata de **adjudicação** é ato **com valor econômico**, cobrado na forma da usucapião enquanto não houver lei estadual | CNN arts. 423 § único e 440-AM | ✅ | F3 |

### Bloco L — Responsabilidade civil, PAD e guarda

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-96 | ⭐ **NÃO existe "a natureza da responsabilidade notarial" — existe a natureza NA DATA DO ATO, em TRÊS faixas.** ① até **21/06/2015**: redação original, **objetiva**, sem prazo próprio na lei especial; ② **22/06/2015 a 10/05/2016**: redação da **Lei 13.137/2015, art. 8º**, ainda **objetiva**, e a única que diz *"temporários ou permanentes"* e alcança *"direitos e encargos **trabalhistas**"* dos prepostos — no intervalo, o **interino** está nominalmente alcançado; ③ a partir de **11/05/2016**: Lei 13.286/2016, **subjetiva** (culpa ou dolo) + **triênio**. **A lei não retroage** — ato de 2014 segue objetivo hoje. **Nunca responder "é subjetiva" sem perguntar a data da lavratura** | Três redações verbatim + prova de vigência de cada uma em `capturas/resp-art22-tres-redacoes-regua-temporal.md`; **REsp 1.849.994** (3ª T., Moura Ribeiro, DJe 24/03/2023 — caso de procuração com assinatura falsa; o tabelião sustentou regime subjetivo e **perdeu**) | ✅ | F4 rev. 2 (⚠️ **corrige a versão anterior deste dossiê, que registrava DUAS faixas**; nem a F2 tinha a do meio) |
| T-96b | **O triênio do art. 22 nasceu SÓ em 2016.** Antes disso a Lei 8.935/94 **não tinha prazo próprio** e a pretensão corria pela regra geral do Código Civil — é por isso que a discussão do termo inicial chegou ao STJ do jeito que chegou (T-97) | Lei 8.935/94, redações 1 e 2 | ✅ | F4 rev. 2 |
| T-97 | **O triênio conta da lavratura pela LETRA, mas o STJ conta do trânsito em julgado da anulatória** quando o dano só se materializa ali (procuração falsa, assinatura falsa, identidade fraudada). Dizer "passaram 3 anos da lavratura, você está seguro" é a resposta que **perde o caso**. Dar as duas datas | Lei 8.935/94, art. 22 § único + **REsp 2.043.325** (3ª T., Nancy Andrighi, notícia oficial 24/08/2023) | ✅ | F4 |
| T-98 | ⭐ **A tese do Tema 777 NÃO usa a palavra "subsidiária"** — ela diz que o Estado responde **objetivamente**, com **dever de regresso** em dolo ou culpa, "sob pena de improbidade administrativa" (arquitetura do art. 37 §6º). **Quem chama a tese de "subsidiária" é o STJ ao aplicá-la** — voto do Min. Moura Ribeiro no REsp 1.849.994: *"a tese fixada pelo STF diz respeito à responsabilidade civil **subsidiária** do Estado"*. **Regra: citar cada uma com a sua fonte, e nunca atribuir ao STF palavra que não está na tese.** A ilegitimidade passiva do titular é **controvérsia**, não certeza — e **na prática ele é réu direto**: no REsp 1.849.994 a ação foi contra o tabelião, o primeiro grau condenou, o TJDFT **aumentou** a condenação e o STJ negou provimento | **RE 842.846/SC**, Pleno, Fux, 27/02/2019, trânsito 19/08/2020, tese verbatim em `capturas/resp-stf-tema-777-verbatim.md` + voto do STJ no REsp 1.849.994 | ✅ (as duas fontes) / 🟡 (a controvérsia de legitimidade, noticiada) | F4 rev. 2 (⚠️ **corrige a versão anterior deste dossiê**, que dizia que a meta "não confere com o Tema 777" — era forte demais: a meta acertou o rótulo que a jurisprudência usa e errou só em apresentá-lo como texto do STF) |
| T-99 | **A serventia não é parte.** Cartório não tem personalidade jurídica nem capacidade processual: responde **a pessoa do titular à época do ato**, e a responsabilidade **não se transmite ao sucessor** na delegação | STJ **REsp 1.097.995** (3ª T., 06/10/2010) e **AREsp 1.858.938** (1ª T., 01/07/2022); Enunciado 77 da I Jornada Notarial e Registral do CJF (doutrina) | ✅ | F4 |
| T-100 | **O foro da ação de reparação é a sede da serventia**, afastado o art. 101, I do CDC por especialidade. É a **primeira defesa processual** de todo titular demandado fora da comarca | CPC art. 53, III, "f" + STJ **REsp 2.011.651** (4ª T., 11/12/2024) | ✅ | F4 |
| T-101 | **As penas são repreensão, multa, suspensão e perda da delegação.** Não existem "advertência" nem "censura" na Lei 8.935/94. E escrever **"90 dias, prorrogável por mais 30"**, não "120 dias" — a fórmula legal preserva a informação de que a prorrogação é ato próprio, que precisa de motivação | Lei 8.935/94, art. 32 | ✅ | F4 (a meta já acertava a nomenclatura; erra na aritmética em uma das seções) |
| T-102 | **NÃO existe prazo prescricional de PAD na Lei 8.935/94.** Aplicam-se os prazos da **legislação estadual de servidores** — **não** a Lei 8.112/90. **Nunca escrever "prescreve em X anos" como regra nacional**: os 2 anos do caso julgado são do **Rio de Janeiro** (DL estadual 220/1975). É a defesa que mata o processo antes do mérito | **STJ, RMS 72.379**, 1ª T., Regina Helena Costa, 14/05/2024 | ✅ | F4 |
| T-103 | **PAD não corre pelo CPC.** É procedimento correcional instaurado e decidido pelo **juízo corregedor competente**, com ampla defesa legal — sem petição inicial, contestação ou revelia. E a Lei 8.935/94 **não regula o rito**: prazo de defesa, instrução e recurso vivem nas **Normas de Serviço da CGJ de cada estado** — 27 ritos. Descrever o PAD com vocabulário de processo civil é erro de produto | Lei 8.935/94, arts. 34-37 | ✅ | F4 |
| T-104 | **A pena não segue ordem de gradação, mas segue proporcionalidade.** O art. 34 dispensa a ordem "conforme a gravidade do fato" — o que **exige correlação** entre pena e fato, e é por aí que se ataca suspensão aplicada sobre falta que o art. 33 tipifica como leve. E **quem impõe a pena é o juízo**, não a corregedoria administrativa isoladamente | Lei 8.935/94, arts. 33 e 34 | ✅ | F4 |
| T-105 | **Perda da delegação: art. 35, I *ou* II — vias autônomas, não sequência.** Sentença transitada **ou** PAD; nenhuma exige a outra. E a **suspensão do §1º corre antes da decisão final** — é o verdadeiro ponto de dor | Lei 8.935/94, art. 35 | ✅ | F4 |
| T-106 | **A suspensão preventiva trava metade da renda líquida por até 120 dias** (90 + 30), com a outra metade em conta especial corrigida: absolvido, o titular recebe; condenado, o montante cabe ao interventor. É o momento de maior dor econômica — e a camada de defesa que não o cobrir cobre a parte errada | Lei 8.935/94, art. 36 e §§ | ✅ | F4 |
| T-107 | **Descumprir a gratuidade da Lei 9.534/97 é hipótese AUTÔNOMA de extinção da delegação** — casa com o art. 31, III (cobrança indevida). Uma serventia de RCPN que erra sistematicamente a gratuidade está a um PAD da extinção | Lei 8.935/94, arts. 39, VI e 45 | ✅ | F4 |
| T-108 | **O art. 103-B, §4º, III da CF está na redação da EC 103/2019 — SEM "aposentadoria com subsídios ou proventos proporcionais".** A redação da EC 45/2004, que ainda circula em manuais e cursinhos, está **superada**. E a competência do CNJ é **CONCORRENTE**, não subsidiária: "sem prejuízo da competência disciplinar dos tribunais", podendo **avocar processos disciplinares em curso**. Um mesmo fato pode ser apurado nas duas instâncias | CF art. 103-B, §4º, III | ✅ | F4 |
| T-109 | **Não existe súmula nem repetitivo do STJ sobre responsabilidade notarial** (nada localizado — ausência declarada, não prova de inexistência). O vinculante é o **Tema 777 do STF**. E **Enunciado de Jornada do CJF é DOUTRINA**, não súmula nem tese — citar com o rótulo certo | base de Enunciados Científicos do STJ | ✅ (o rótulo) / 🔴 (a ausência) | F4 |
| T-110 | **A Tabela de Temporalidade mudou em 26/11/2024:** depósito de firmas, reconhecimento de firma **por autenticidade** e fichas de depósito deixaram de ser **Permanente** e passaram a **5 anos** — **condicionado à digitalização com valor legal**. Descartar sem a digitalização conforme é infração, não economia. Um plugin treinado antes dessa data responde "Permanente" e está errado | **Prov. CN n. 185, de 26.11.2024**, sobre o Prov. CNJ 50/2015; Lei 12.682/2012, art. 2º-A + Decreto 10.278/2020 | ✅ | F4 |
| T-111 | **A guarda dos documentos que instruíram escritura e procuração é de 10 ANOS** — o CNJ ancorou no **art. 205 do CC**, não no triênio do art. 22. **Nunca sugerir descarte no prazo mínimo do que instruiu ato de alto risco: o prazo de guarda é o prazo em que você ainda tem defesa** (coerente com a *actio nata* da T-97) | Prov. CNJ 50/2015, cód. 3-5-5; adoção tornada obrigatória pelo **CNN art. 196** | ✅ | F4 |
| T-112 | **Descarte tem rito:** o documento deve ser **desfigurado** de modo que as informações não possam ser recuperadas, e **toda eliminação é comunicada SEMESTRALMENTE ao juízo competente**. A eliminação não afasta os deveres da LGPD quanto aos dados que remanescerem em índices e bancos | Prov. CNJ 50/2015, arts. 2º e 3º; CNN art. 92 | ✅ | F4 |
| T-113 | **Perícia sobre o acervo é NA SEDE da serventia, com ciência do titular e autorização do juízo.** Remoção de livro sem isso é nulidade da prova — defesa pura que quase ninguém invoca | Lei 8.935/94, art. 46 § único | ✅ | F4 |
| T-114 | **Incidente com dados pessoais: 48 HORAS ÚTEIS** do conhecimento, comunicando ao titular dos dados, à **ANPD**, ao **juiz corregedor permanente** e à **CGJ**. Prazo curtíssimo e gatilho disciplinar quando descumprido | CNN art. 91 | ✅ | F4 |
| T-115 | **A correição é ANUAL e previsível**, e verifica a adaptação das práticas de tratamento de dados à LGPD e ao Código — o que a torna o melhor alvo de produto preventivo que existe | CNN art. 105 | ✅ | F4 |
| T-116 | **Papel de segurança tem numeração nacional única e irrepetível**, com Código de Verificação Digital de consulta pública, e **é vedada a alienação ou cessão de papel entre serventias, "sob pena de responsabilidade civil, penal e administrativa"**. O controle de faixa numérica é prova de rastreabilidade — a ausência dela sustenta acusação de extravio | CNN arts. 64-A a 64-I (Prov. CN 211, de 28.1.2026) | ✅ | F1, F2, F4 |
| T-117 | **Não existe nota devolutiva federal para o tabelião de notas.** Para o registrador o caminho é normatizado (nota devolutiva + dúvida, LRP 198-204; e no protesto, art. 395 do CNN exige recusa "por escrito, com exposição de seus fundamentos"). Para notas, **não há equivalente** — ele simplesmente não lavra. O instrumento é **estadual**, e o controle é do juiz corregedor + CNJ | varredura das 369 pp. + LRP 198-204 | ✅ | F2, F4 |
| T-118 | **Exigência sem os três elementos é o que o CNJ anulou duas vezes em 2025.** Toda nota fundamentada deve citar: (i) o **dispositivo legal** que sustenta a exigência; (ii) a **razão concreta** no caso; (iii) o **caminho de correção** | PCA 0001611-12 e PCA 0007885-89, ambos rel. Cons. Marcello Terto | ✅ (os precedentes) / 🟡 (a regra de desenho) | F2 |
| T-119 | **O art. 21 é arma de dois gumes.** É o argumento comercial (só o titular decide contratar) **e** o argumento acusatório no PAD: a organização do serviço é responsabilidade **exclusiva** dele, e "foi o escrevente" não é defesa. Quem autoriza escrevente a praticar ato de alto risco sem trilha documental está construindo a própria condenação | Lei 8.935/94, arts. 20 e 21 | ✅ | F4 |
| T-120 | **Desqualificada a escritura no RI, o tabelião NÃO precisa assistir calado:** o juízo da dúvida pode admitir a **intervenção espontânea do tabelião que lavrou a escritura** objeto da desqualificação. **Enunciado de Jornada é doutrina orientadora**, não súmula | Enunciado 76 da I Jornada de Direito Notarial e Registral do CJF | ✅ (o enunciado) / 🟡 (o efeito) | F4 |

### Bloco M — Regulação de IA em serventia (a camada nova)

| # | Trava | Dispositivo / fonte | Selo | Origem |
|---|---|---|---|---|
| T-121 | **É VEDADO usar IA para "interpretação normativa, QUALIFICAÇÃO REGISTRAL ou enquadramento legal" de atos** e para a prática **autônoma, total ou parcial**, de ato notarial ou registral | **Prov. TJMT/CGJ n. 1/2026, art. 4º, I e II** | ✅ | F5 |
| T-122 | **É VEDADO usar IA para "tomada de decisão jurídica, inclusive como instrumento de APOIO, SUGESTÃO ou INFLUÊNCIA, direta ou indireta, ainda que sob revisão humana"** — a vedação alcança o modo consultivo, não só o autônomo. É o dispositivo que redefine como o gate de vigência pode ser redigido | Prov. TJMT 1/2026, art. 4º, III | ✅ | F5 |
| T-123 | **É PERMITIDA a "elaboração preliminar de textos e minutas, sob revisão humana"**, a sumarização de documentos públicos, a classificação administrativa, a automação de rotinas operacionais, a análise estatística e **chatbots baseados exclusivamente em dados públicos** — com **supervisão humana obrigatória** e vedação de "qualquer prática que induza a aparência de ato produzido autonomamente" | Prov. TJMT 1/2026, art. 5º e §§ | ✅ | F5 |
| T-124 | **É VEDADO processar documento com dado sigiloso, pessoal, sensível, patrimonial, registral ou notarial em plataforma externa sem anonimização irreversível** — violação é **falha grave de segurança da informação** — e é vedado **treinar ou alimentar modelo com dados do acervo** | Prov. TJMT 1/2026, art. 4º, V e VI, e § único | ✅ | F5 |
| T-125 | **LLM comercial por assinatura é permitido, com SETE condições cumulativas:** capacitação prévia **comprovada documentalmente**; uso estritamente auxiliar; anonimização irreversível; **cláusula contratual expressa** de não-treinamento; **comunicação anual à Corregedoria**; **registro interno das utilizações para auditoria**; e menção expressa do uso de IA com revisão humana integral. A Corregedoria pode **vedar, suspender ou restringir** a solução a qualquer tempo | Prov. TJMT 1/2026, art. 6º e § único | ✅ | F5 |
| T-126 | **Contratar solução de IA exige análise prévia de risco, avaliação de impacto no tratamento de dados, verificação de conformidade e relatório técnico** — e o contrato precisa ter, no mínimo, cláusula de não-treinamento, de não-retenção/não-compartilhamento/não-armazenamento de inputs e outputs, compliance LGPD, mecanismos de auditoria e privacy by design/by default | Prov. TJMT 1/2026, arts. 7º e 8º | ✅ | F5 |
| T-127 | **Serventia vaga (interino) depende de AUTORIZAÇÃO PRÉVIA da CGJ** para usar IA, com justificativa técnica, plano de governança e **"valor compatível com o mercado"** | Prov. TJMT 1/2026, art. 9º | ✅ | F5 |
| T-128 | **A capacitação é obrigatória, com conteúdo definido** (fundamentos e limitações da IA, **riscos de vieses, erros e alucinações**, LGPD, casos práticos, ética, supervisão humana) e **renovação a cada 24 meses** ou a cada mudança tecnológica significativa | Prov. TJMT 1/2026, art. 11, V | ✅ | F5 |
| T-129 | **As sanções chegam a FALTA GRAVE nos termos do art. 31 da Lei 8.935/94** — além de advertência, multa, suspensão imediata da solução, responsabilização civil e comunicação ao CNJ; incidente com dado pessoal vai à **ANPD** | Prov. TJMT 1/2026, art. 14 e § único | ✅ | F5 |
| T-130 | 🔴 **O Prov. TJMT 1/2026 se fundamenta no Prov. CNJ 74/2018 — revogado 28 dias depois** pelo Prov. CNJ 213/2026 (que por sua vez já foi alterado pelo Prov. CN 243, de 21.7.2026). **Reproduzir a remissão do provimento mato-grossense é citar norma revogada** | Prov. TJMT 1/2026 (23/01) × Prov. CNJ 213/2026 (20/02) | ✅ | F5 |
| T-131 | 🟡 **MT é o primeiro, não vai ser o único.** Corregedorias estaduais "passaram a discutir" regulamentação de IA em serventias em 2026. **Vender a norma mato-grossense como se fosse nacional é o erro que a família já pegou em trânsito e criminal** — o produto diz: "em MT já é norma; nas demais UFs é o padrão que está se formando" | Anoreg/RS | 🟡 | F5 |
| T-132 | ✅ **A filosofia standalone-first da família vira vantagem REGULATÓRIA, não só técnica.** Um plugin que roda no ambiente do próprio titular, com a chave dele, sem retenção, é exatamente o desenho que o art. 4º, V e VI e o art. 6º, III e IV exigem — e prova por arquitetura o que um SaaS precisa provar por contrato | Prov. TJMT 1/2026 | ✅ | F5 |

---

## 4. Correções à `PESQUISA-META.md`

Tabela única, consolidando as correções das cinco frentes. **Nenhuma delas invalida a tese central
da meta** (Tabelionato de Notas é a especialidade que paga o plugin — F5 confirmou por dado). Todas
ajustam premissas de fato. Impacto: **alto** = muda arquitetura, posicionamento ou promessa ·
**médio** = muda fronteira ou conteúdo de camada · **baixo** = precisão de citação.

| # | O que a meta afirmava | O que a fonte primária mostrou | Impacto | Frente |
|---|---|---|---|---|
| C-01 | §1.5: "Provimento n. 149/2023 (CNN), **4.9.2023**" | O ato é de **30.8.2023**; 4.9.2023 é a **publicação** (DJe/CNJ 207/2023) | Baixo | F1 |
| C-02 | §1.5: "Parte Geral com **5 Livros**" | São **6** — o Livro VI foi acrescido depois | Baixo | F1 |
| C-03 | §1.5: "**60+ alterações**" | São **57** | Baixo | F1, F3 |
| C-04 | §1.5: "a mais recente rastreada: **Prov. 246/2026** (28.7.2026)" | Correto na data da meta; hoje é o **Prov. 253, de 18.8.2026** | Médio (é gate, não curiosidade) | F1, F2, F3 |
| C-05 | §1.5: "**Provimento 244/2026** (21.7.2026)" como alteração do CNN | **Errado nos dois campos.** A alteração de 21.7.2026 é o **242**; o **244 é de 22.7.2026** e trata de passivos funcionais da magistratura | Médio | F1 |
| C-06 | §1.5: o Prov. 149/2023 "**absorveu todos** os provimentos anteriores"; provimentos antigos "hoje são **remissão histórica, não a norma vigente**" | **Verdadeiro só para trás e só para a Corregedoria.** Seis provimentos notarialmente relevantes seguem **vivos por remissão** (56/2016 RCTO, 103/2020 AEV, 62/2017, 50/2015, 197/2025, 213/2026); há **dois regimes** pós-149 (alterador × autônomo); e as **Resoluções do Plenário nunca foram absorvidas** — terceiro endereço. Tratá-los como remissão histórica faz o plugin **ignorar norma aplicável** | **Alto** | F1, F3 |
| C-07 | §1.5: "172/2024 e 175/2024 suspensos por Pedido de Providências **ainda em trâmite**" | Suspensão confirmada e **ainda formalmente vigente na ficha**, mas o PP **não está mais em trâmite** — foi **julgado procedente em 24.7.2026**, e o **Prov. 246, de 28.7.2026** reescreveu o art. 440-AO em sentido **oposto**. Há ainda **um terceiro suspenso** que a meta não conhecia: o **Prov. 247/2026** (VNS), suspenso em 13.8.2026 | **Alto** | F1 |
| C-08 | §7.1: o esqueleto abre "o livro do Tabelionato de Notas" | O Livro IV da Parte Especial é **residual** (arts. 441-444-G, três dos cinco capítulos são remissões puras). O **núcleo está na Parte Geral, Livro IV, Cap. VI, arts. 264-319**. Um plugin que abra o livro de notas **perde o e-Notariado inteiro** | **Alto** | F1 |
| C-09 | §1.6: linha da **Lei 14.382/2022** atribui a ela o "art. **7º-A**" (mediação/conciliação/arbitragem) | O art. **7º-A inteiro é da Lei 14.711/2023**. Da 14.382/2022 são **só os §§ 1º a 5º do art. 7º**. A meta se contradiz na linha seguinte — é exatamente a confusão que ela manda evitar | **Alto** | F3 |
| C-10 | §1.6: linha da **Lei 14.711/2023** — "arts. 6º-A/7º-A (cessão de precatório)" | Impreciso: **6º-A = precatório**; **7º-A = condição negocial + mediação/conciliação + arbitragem + conta vinculada** | Médio | F3 |
| C-11 | §7.1 põe **execução extrajudicial de hipoteca** na Camada 2 (Registro de Imóveis) | **Não é registral.** A Lei 14.711/2023, art. 9º, **§11** manda os autos a **tabelião de notas** para a **ata notarial de arrematação**, que **"constituirá título hábil de transmissão da propriedade"**. É o **único** ato notarial desta onda que é título translativo | **Alto — muda a arquitetura de camadas** | F3 |
| C-12 | §1.3: 216-B exige "notificação prévia do inadimplente (15 dias)" | Correto no prazo, **mas a notificação é do OFICIAL DO RI** (que pode delegar ao RTD) — art. 216-B, §1º, II. **Não é ato do tabelião de notas** | Médio (fronteira) | F3 |
| C-13 | §1.6 descreve a **Res. 571/2024** como incapaz + testamento + alienação pelo inventariante + união estável | **Incompleto.** Faltam: divórcio com filho menor/incapaz (34 §2º); escrituras de **separação de fato** e de **restabelecimento da comunhão plena de vida** (52-A a 52-E, **figuras que não existiam**); **certidão por quesitos** (3º § único); revogação dos arts. 45 e 47. São **atos novos vendáveis** que a meta não viu | **Alto** | F3 |
| C-14 | §7.1 não menciona **conta notarial vinculada** nem **RCTO/CENSEC** | **Prov. CNJ 197/2025** (vigente, ancorado no CNN art. 444-G pelo Prov. 202/2025) traz o **único rol de recusa obrigatória**; e o **CNN art. 441, II** torna a consulta ao RCTO **obrigatória** antes do inventário | **Alto** | F2, F3 |
| C-15 | §§2 e 5: arbitragem notarial como "produto novo de 2023 que ainda não tem ferramenta dedicada" | Verdade, **e mais grave: não tem RITO.** Zero ocorrência de `árbitro/arbitragem/arbitral` no CNN inteiro. E §7.1 trata "mediação/conciliação/arbitragem" como **uma** skill — são **três regimes distintos**, sendo que mediação e conciliação dependem de **autorização prévia da CGJ/Nupemec** | **Alto** | F1, F3 |
| C-16 | §1.2: "art. 8º — livre escolha do tabelião de notas" | **Não sobrevive no ato eletrônico**, onde a competência é **exclusiva e ABSOLUTA** por circunscrição (CNN 289, 302-304). Um plugin que ensinasse "art. 8º, sempre" produziria escritura eletrônica lavrada por tabelião incompetente — e competência absoluta violada é vício de origem | **Alto** | F2 |
| C-17 | §§1.2 e 3.1: "responsabilidade civil **subjetiva**", **sem recorte temporal** | ⭐ **A pergunta "qual é o regime?" é malformada — a correta é "de que data é o ato?".** São **TRÊS** faixas, não duas: objetiva até 21/06/2015 · objetiva pela **Lei 13.137/2015** entre 22/06/2015 e 10/05/2016 (a única que alcança "temporários ou permanentes" e encargos **trabalhistas** dos prepostos) · subjetiva + triênio a partir de 11/05/2016. **A faixa do meio não estava registrada em lugar nenhum** — nem na meta, nem no briefing, nem no apontamento da F2, que corretamente via duas | **Alto** | F4 rev. 2 |
| C-18 | §3, item 2: "Responsabilidade do Estado é **subsidiária**, não solidária — o titular responde primeiro" | ⚠️ **Correção mais fina do que a primeira leitura sugeria.** A tese literal do STF **não emprega** a palavra "subsidiária" — ela fixa responsabilidade **objetiva** com dever de regresso. **Mas o STJ chama-a exatamente disso** ao aplicá-la (voto do Min. Moura Ribeiro no REsp 1.849.994). ⇒ **A meta acertou o rótulo que a jurisprudência usa e errou só em apresentá-lo como se fosse texto do STF.** A regra do plugin não é "a meta está errada", é: **nunca atribuir "subsidiária" à tese do STF, e citar cada fonte com o seu rótulo** | **Alto** | F4 rev. 2 (⚠️ **corrige a versão anterior deste dossiê**, que classificava a frase da meta como simplesmente errada) |
| C-19 | Trava 6 (§7.2): "prescreve em 3 anos da **lavratura**, não da descoberta" | **Certa quanto à letra da lei, incompleta quanto ao risco real.** O STJ aplica *actio nata* quando o dano só se define com a **anulação judicial** (REsp 2.043.325). Sem o complemento, a trava produz a resposta errada no caso mais comum: fraude documental | **Alto** | F4 |
| C-20 | §3, item 3: "suspensão até **120 dias**" | A lei diz **"noventa dias, prorrogável por mais trinta"** (art. 32, III). A própria meta usa a fórmula legal em §1.2 e a aritmética em §3 — preferir a legal | Baixo | F4 |
| C-21 | §3 trata o **PAD** como se o rito fosse federal | **Não é.** A Lei 8.935/94 não regula rito **nem prazo prescricional** (STJ RMS 72.379: aplica-se a lei **estadual** de servidores, não a 8.112/90). São **27 ritos** e 27 prazos. Isso põe o PAD na mesma categoria dos emolumentos — a meta lista só emolumentos ali; **são dois** (e F2 acrescenta o terceiro: a recusa em notas) | **Alto** | F4 |
| C-22 | §4: "cada uma podendo usar valor fixo, **percentual sobre o negócio**, ou faixa" | **Lei 10.169/2000, art. 3º, II: é VEDADO fixar emolumentos em percentual sobre o valor do negócio.** A estrutura legal é faixa (2º III b) ou valor por espécie (2º III a). O único percentual federal é o **teto** de 0,3% do crédito rural | **Alto — ensinaria prática vedada ao próprio delegatário** | F5 |
| C-23 | §4 e trava 4: "**27 tabelas estaduais**" / "emolumento é lei estadual" | **26 leis estaduais + 1 lei FEDERAL** (DF, Lei 14.756/2023). E cada UF tem **várias** tabelas — SP tem cinco. A trava "confira a tabela do seu estado" **quebra no DF** | Médio | F5 |
| C-24 | §5 e Resumo 6(c): "o que existe hoje — IARI, Escriba, Officer Soft — é *gestão de serventia*, **não redação/qualificação assistida**"; "**isso é o espaço aberto**" | **Falso, e a inversão é o achado comercial mais duro.** A **IA Not** do **CNB/CF** (set/2025), dentro do e-Notariado, faz "apoio na redação de minutas"; o **AryaBolt** (preço público R$ 449-1.349/mês) promete "automação completa na elaboração de escrituras, procurações, testamentos e atas notariais". **Ambos anteriores a 18/08/2026** — não é o mercado que se moveu, foi a varredura que não os alcançou | **Alto — muda o posicionamento inteiro** | F5 |
| C-25 | §5: "**~13.440 cartórios** (dado 2024, 6ª edição)" | A edição corrente é a **7ª/2025**, e publica **12.210** serventias — corroborado internamente pela contagem de titulares (6.193 + 5.950 + 67 = 12.210, fonte Justiça Aberta/CNJ). A mesma edição usa **12.512** em outro capítulo: a própria Anoreg é **internamente inconsistente** | Médio | F5 |
| C-26 | §5: 🔴 "não confirmado o split exato por especialidade" | **Fechado:** Notas = **8.228** (67,4% das serventias), RCPN 7.201, Protesto 3.846, RTD/RCPJ 3.810, RI 3.682, RCM 556, RD 347. A soma (27.670) excede o total porque **uma serventia acumula atribuições** | Médio (fecha um 🔴 da meta) | F5 |
| C-27 | A meta **não menciona regulação de IA em cartório** | **Res. CNJ 615/2025 · Prov. CNJ 213/2026** (revoga o 74/2018, já alterado pelo 243/2026) **· Prov. TJMT 1/2026**, que **veda nominalmente** "qualificação registral" por IA e **autoriza** "elaboração preliminar de minutas sob revisão humana" | **Máximo — redesenha o esqueleto §7.1 e cria uma camada de produto nova** | F5 |
| C-28 | §1.5 e trava 1: "citar provimento pelo número antigo sem apontar a absorção é erro" | Correto — **e o próprio Código faz remissão nominal a provimento antigo** (art. 441, II cita o "Provimento n. 56, de 14 de julho de 2016"). A trava não é só "não cite provimento velho", é "**siga a remissão que o Código faz**" — senão o validador gera falso-positivo | Baixo (evita falso-positivo) | F3 |
| C-29 | A meta **não registra a tensão CPC × Resolução** | CPC arts. 610 *caput* e 733 *caput* **contra** os arts. 12-A, 12-B e 34 §2º da Res. 35/2007. Quem abriu as hipóteses foi uma **Resolução**, não uma lei — e é isso que o titular vai alegar num PAD | **Alto — é a postura honesta do produto** | F3 |
| C-30 | A meta **não conhece** a Lei 7.433/85 nem o Decreto 93.240/86 | São a **espinha dorsal documental** da escritura de imóvel — o Decreto traz o **rol FECHADO**, o prazo de 30 dias da certidão do RI e a dispensa das fiscais pelo adquirente. Sem eles, uma skill de escritura **teria de inventar o checklist** | **Alto** | F2 |

### 4.1 Divergências ENTRE FRENTES — resolvidas e não resolvidas

**Resolvidas pela fonte (registro para rastreabilidade):**

| Divergência | Resolução | Fonte que decidiu |
|---|---|---|
| **F5 §2.3** afirmou que o **Provimento CNJ 150/2023** (adjudicação compulsória) é **posterior ao 149/2023 e vige em separado** — contradizendo a premissa da meta. **F3 §1.1** foi à fonte e provou que ele é um provimento **ALTERADOR**: ementa *"**Altera** o Código Nacional de Normas… instituído pelo Provimento nº 149"* e art. 1º *"passa a vigorar **acrescido do seguinte Capítulo V**"* | **F3 vence — fonte mais forte** (ementa e art. 1º verbatim, `atos.cnj.jus.br/atos/detalhar/5258`). O conteúdo do 150/2023 **é** o CNN, arts. 440-A a 440-AM. Citar "Prov. 150/2023, art. 5º" erra o endereço. **Mas F5 acertou o principal:** "tudo virou 149/2023" é regra falsa — só que por outro motivo (provimentos **autônomos** + Resoluções do Plenário) | F3 ✅ |
| **F4 §8.5** registrou discrepância entre a meta e a tabela da ANOREG nas datas dos Provimentos 242/244 e 228/229, sem resolver (declarou "é a frente F1") | **F1 §2 resolveu:** a alteração de 21.7.2026 é o **242** (o 244 é de 22.7 e é da magistratura); e os Provimentos **228 e 229 existem os dois**, ambos de 16.6.2026 | F1 ✅ |
| **F1 §4.1** descreve o Livro IV da Parte Especial como "**residual**, cinco capítulos, três dos quais remissões puras". **F2 §4** afirma que ele "**não é puramente residual**" | **Reconciliável, não é contradição:** os dois concordam na estrutura. F1 mede a proporção (3 de 5 capítulos são remissões); F2 observa que os **arts. 444-A a 444-G são camada nova** (AEDO/2024, conta notarial/2025). A leitura consolidada é a de T-14 + T-14b | ambas ✅ |

**NÃO resolvidas — registradas como divergência aberta:**

| # | Divergência | Por que não resolvi | Impacto |
|---|---|---|---|
| **D-1** | **O que contém o campo "Alteração" da ficha do CNN.** **F1 §2** afirma ter extraído programaticamente **57 itens da lista oficial**, com controle negativo. **F3 §0.8** afirma que a lista traz **49**, o corpo consolidado traz **53**, e que as duas **não se contêm** (8 só no corpo, 4 só na lista), somando 57 na união | As duas frentes chegam ao **mesmo total (57)**, mas descrevem conteúdos diferentes para a mesma lista. Não consigo decidir sem reabrir a ficha — e não pesquiso | **Baixo no número, MÉDIO na rotina de refresh:** se F1 estiver certa, vigiar a lista basta; se F3 estiver certa, é **obrigatório cruzar lista × corpo**. **Adotar o procedimento mais conservador (cruzar) é seguro nos dois cenários** |
| **D-2** | **Contagem de ocorrências de "ata notarial" no CNN:** F1 §4.2 diz **22**; F2 §4.0 diz **21** | Diferença de método de contagem (provavelmente inclusão ou não da Exposição de Motivos) | **Nulo para o produto** — as duas concordam no fato estrutural: **não existe capítulo geral de ata notarial no CNN**. Registrado só por honestidade |
| **D-3** | **Parâmetro remuneratório da mediação notarial:** CNN art. 52 (tabela de escritura **SEM** valor econômico) × Lei 8.935/94, art. 7º-A §3º (tabela **COM** valor econômico) | **Não é divergência entre frentes — é conflito dentro da própria norma**, levantado por F3 §5.2 e não resolvido pela fonte (regulamentar-supletivo × legal-supletivo) | **Médio** — a skill de mediação precisa declarar o conflito e remeter à norma estadual, nunca escolher um dos dois em silêncio |
| **D-4** | **Data da liminar que suspendeu os Provimentos 172 e 175:** fontes secundárias divergem entre **27** e **28/11/2024** | Divergência entre fontes secundárias, não entre frentes. A ficha do CNJ não publica a data | **Baixo** — não citar a data da liminar; citar a **suspensão** e o desfecho de 24.7.2026 |

---

## 5. Regulação de IA em serventia — a camada nova (F5)

A meta-pesquisa não a viu. Ela existe, tem prazo, tem sanção, e **redesenha o produto**: um plugin
de IA vendido a cartório em 2026 é, ele próprio, objeto de norma.

### 5.1 A pirâmide

```
Resolução CNJ n. 615/2025 — IA no Judiciário (governança, classificação de risco,
   │                        vedações à IA generativa em atividades sensíveis, supervisão humana)
   │
   ├─ Provimento CNJ n. 213, de 20/02/2026 — padrões mínimos de TI e segurança da informação
   │    nas serventias extrajudiciais. REVOGOU EXPRESSAMENTE o Provimento CNJ 74/2018.
   │    Já alterado pelo Provimento CN n. 243, de 21/07/2026.
   │
   └─ Provimento TJMT/CGJ n. 1/2026-GAB-CGJ (23/01/2026) — PRIMEIRA norma estadual do país
        sobre IA dentro de serventia extrajudicial. Vigência: 90 dias após a publicação.
```

Captura verbatim: `pesquisa/capturas/mercado-provimento-tjmt-1-2026-ia-serventias.md` ✅

### 5.2 O que é VEDADO (art. 4º, "em qualquer modalidade")

| Inciso | Vedação | Por que importa ao produto |
|---|---|---|
| I | Prática **autônoma, total ou parcial**, de ato notarial ou registral | Nenhuma skill pode "praticar o ato" |
| **II** | **Substituição da análise jurídica humana, inclusive quanto a interpretação normativa, QUALIFICAÇÃO REGISTRAL ou enquadramento legal** | **Vedação nominal** — atinge a skill `qualificacao-registral-e-duvida` do esqueleto pelo nome e pela promessa |
| **III** | Valoração de provas, identificação de perfis, predição de comportamento ou **tomada de decisão jurídica, inclusive como instrumento de APOIO, SUGESTÃO ou INFLUÊNCIA, direta ou indireta, ainda que sob revisão humana** | **É o dispositivo mais largo da norma.** Alcança o modo consultivo, não só o autônomo — e é ele que decide como o gate de vigência pode ser redigido |
| IV | Reconhecimento facial, biométrico ou emocional, salvo autorização expressa do CNJ | Fecha a porta a qualquer feature de identificação por imagem |
| **V** | Processar documento com **dado sigiloso, pessoal, sensível, patrimonial, registral ou notarial em plataforma externa, sem prévia anonimização irreversível** — § único: é **falha grave de segurança da informação** | Ataca frontalmente o SaaS que sobe acervo |
| VI | **Treinamento**, aperfeiçoamento, retenção ou alimentação de modelos com dados do acervo | Idem |

### 5.3 O que é AUTORIZADO (art. 5º, baixo risco, fins auxiliares)

I sumarização de documentos públicos · **II elaboração preliminar de textos e MINUTAS, sob revisão
humana** · III classificação administrativa de documentos · IV automação de rotinas meramente
operacionais · V análise estatística para gestão · **VI chatbots informativos baseados
exclusivamente em dados públicos** · VII formatação e organização textual.

**§1º** supervisão e revisão humana **obrigatórias**, com o delegatário respondendo pelo conteúdo
final. **§2º** — *"vedada qualquer prática que induza a aparência de ato produzido autonomamente"*.

E o **art. 6º** autoriza expressamente **LLM comercial por assinatura privada** para as atividades
do art. 5º, cumpridas **sete condições cumulativas** (T-125).

### 5.4 O que isso OBRIGA a mudar na redação das skills

Cinco consequências diretas, todas de F5 §5.3:

1. **`qualificacao-registral-e-duvida` não pode ser vendida com esse nome nem com essa promessa.**
   "Qualificação registral" é vedação nominal (art. 4º, II). O que a norma permite é **checklist de
   exigências + minuta preliminar de nota devolutiva, sob revisão humana** (art. 5º, II) — *o titular
   qualifica, o plugin organiza*. **É reescrita de posicionamento, não de escopo.**
2. **O gate de vigência muda de verbo.** Se ele **decide** se o ato pode ser lavrado, cai no art. 4º,
   III (apoio/sugestão/influência, ainda que sob revisão humana). Se ele **exibe a norma vigente com
   fonte e data** e deixa a decisão ao titular, é art. 5º, I e VII. **A diferença está na redação da
   skill, não na sua função.**
3. **O verbo certo atravessa o produto inteiro.** O padrão normativo que emerge de F3 §9 é o mesmo:
   o delegatário **não julga o mérito — ele verifica, documenta e devolve ao juízo**. Os três verbos
   que mais se repetem no corpo normativo são **"encaminhar ao juízo/MP"**, **"fundamentar por
   escrito"** e **"consignar no ato"**. Uma skill escrita nesses verbos está simultaneamente correta
   pela postura do delegatário **e** dentro do art. 5º. Uma skill escrita em "decida", "recomendo",
   "o entendimento é" viola as duas coisas ao mesmo tempo.
4. **Nenhuma saída pode "induzir a aparência de ato produzido autonomamente"** (art. 5º §2º) — toda
   minuta sai marcada como **preliminar, sujeita a revisão humana integral**, e com **menção expressa
   do uso de IA** quando relevante (art. 6º, VII).
5. **A arquitetura standalone-first da família vira argumento regulatório.** Rodar no ambiente do
   titular, com a chave dele, sem retenção nem treinamento, é exatamente o desenho que os arts. 4º
   (V e VI) e 6º (III e IV) exigem. O concorrente SaaS precisa **provar por contrato** o que o plugin
   **prova por arquitetura** (T-132).

**E uma trava sobre a própria norma:** o Prov. TJMT 1/2026 se fundamenta no **Prov. CNJ 74/2018**,
revogado **28 dias depois** pelo Prov. CNJ 213/2026 (T-130). E MT é o primeiro, **não é nacional**
(T-131) — vender a norma mato-grossense como se valesse no país inteiro é o erro que a família já
pegou em trânsito e criminal.

### 5.5 A consequência do botão P-1 — a camada vira o diferencial central

O Doc cravou: **esta camada entra no v0.1 como diferencial central**, não como apêndice. Os seis
artefatos, com o dispositivo que cobra cada um, estão em **§2.2-bis**. O que esta seção acrescenta é
o **porquê comercial** e a **honestidade obrigatória**:

**Por que ela sustenta a oferta melhor que a redação de minuta** — três razões que saem da própria
pesquisa, não de intuição:

1. **Ninguém vende isso.** O AryaBolt cita o Prov. 213 como selo de conformidade; **nenhum player
   entrega os artefatos** (F5 §3.4.1 ✅). A IA Not resolveu o problema de LGPD **para si mesma**, por
   contrato com os motores — o que não produz um único documento que o titular possa mostrar à
   Corregedoria dele.
2. **Tem prazo legal correndo e sanção que chega a falta grave** (art. 17: 90 dias para quem já usa
   IA; art. 14, VI: falta grave do art. 31 da Lei 8.935/94). **Necessidade com prazo tem
   elasticidade baixa** — é o argumento de preço mais forte que a pesquisa produziu (F5 §6.3).
3. **A arquitetura standalone-first da família é a prova, não a promessa.** Rodar no ambiente do
   titular, com a chave dele, sem retenção nem treinamento, é literalmente o desenho que os arts. 4º
   (V e VI) e 6º (III e IV) exigem. O SaaS **prova por contrato**; o plugin **prova por
   arquitetura** (T-132 ✅).

**E a honestidade que a camada é obrigada a carregar (F5, 🟡):** **só MT regulou até agora.** A
frase do produto é *"em MT já é norma; nas demais UFs é o padrão que está se formando"* — nunca
"conformidade nacional". Duas consequências práticas disso: (a) fora de MT, os seis artefatos valem
como **boa prática antecipatória**, e é assim que devem ser vendidos; (b) o `context/` precisa de um
**mapa de normas estaduais de IA por UF com data de corte**, e F5 avisa que é *"o `context/` que mais
vai envelhecer"* — o que liga esta camada direto ao requisito de arquitetura da §7.6.

---

## 6. Concorrência e posicionamento

### 6.1 Quem existe (F5 §3)

| Player | O que é | Faz redação/qualificação assistida? | Preço | Selo |
|---|---|---|---|---|
| **IA Not — CNB/CF** ⭐ | Desenvolvimento **interno do Colégio Notarial do Brasil**, rodando **dentro do e-Notariado**, sobre "motores de grandes empresas de IA no mercado global" sob contrato do CNB. Lançada no Encontro Notarial do Sudeste, **set/2025** | **SIM** — preenchimento automático de campos do ato eletrônico, **"apoio na redação de minutas e documentos"**, resumos para conferência, verificação e cruzamento de dados. Roadmap declarado: **"propor minutas de atos notariais e de instrumentos particulares"** | Não anunciado — 🟡 tudo indica **embutido no e-Notariado** | ✅ (entrevista oficial, 29/09/2025) |
| **AryaBolt (nTask)** ⭐ | "Primeira solução híbrida SaaS/TaaS criada exclusivamente para o ecossistema notarial e registral brasileiro". Sede Palmas-TO | **SIM** — módulo Notas: *"automação completa na elaboração de escrituras, procurações, testamentos e atas notariais com assistente de redação jurídica inteligente"*; módulo RI: *"qualificação registral automatizada"* ⚠️ (promessa que colide com o art. 4º, II do Prov. TJMT) | **R$ 449 / 649 / 949 / 1.349 por mês**; @Bolt (escrevente virtual com RAG isolado por cartório) **R$ 49/mês + tokens** | ✅ (página e preços públicos) |
| **@Arya** | Assistente notarial/registral **pública e GRATUITA no WhatsApp**, do mesmo fornecedor: "responde de forma estruturada, citando as leis vigentes e provimentos do CNJ" | É consulta normativa pura | **Grátis** | ✅ |
| **IARI (ONR + Google)** | Extração de dados de matrícula por OCR/IA no Registro de Imóveis | **Não** — só extração de dado existente, e **só RI** | — | ✅ |
| **Escriba Informática** | ERP notarial/registral | **Não comprovado** — a página de IA **retorna 404** | — | 🟡 (404 verificado) |
| **Officer Soft ("Smart Officer")** · **Siplan** · **ialocus** | ERPs de cartório com discurso de IA em gestão/BI | 🟡 escopo de redação **não declarado publicamente** | — | 🟡 |
| **MinutaIA** | IA jurídica para minutas, petições e sentenças (Judiciário e advocacia) | **Não é do domínio** — adjacente, não concorrente | — | ✅ |
| **Smart Escritura (CNB/CF, 2023)** | Antecedente do mesmo ator: "escritura inteligente" com IA em blockchain, lançada no Encontro Mundial do Notariado | — | — | ✅ |

🔴 **"3.516 Cartórios Conectados" e "38% de satisfação"** são contadores animados na landing do
AryaBolt, sem auditoria e sem eco em nenhuma cobertura setorial. 3.516 seria ~29% de todas as
serventias do país. **Marketing, não dado.**

### 6.2 O que já está ocupado

**O espaço "assistente que redige a minuta padrão" está ocupado, provavelmente de graça, pela
entidade de classe do próprio comprador.** O CNB/CF está **dentro da ferramenta que o tabelião já é
obrigado a usar** (CNN art. 284 § único: "todos os tabeliães **deverão** prestar o serviço"), e já
resolveu por contrato o problema de LGPD que o Prov. TJMT 1/2026 impõe a qualquer solução externa.
Um plugin comercial não ganha desse no terreno "preencher campo e propor minuta padrão" — F5 §3.1.

**E uma fresta sumiu:** "consulta de norma notarial" pura. A **@Arya é gratuita, no WhatsApp, 24h**.
Não construir camada cujo valor único seja responder pergunta de direito notarial — está
commoditizado desde antes desta pesquisa (F5 §3.4).

### 6.3 As frestas que sobram

**Três frestas que F5 nomeou:**

1. ⭐ **Conformidade regulatória de IA** — os artefatos do Prov. TJMT 1/2026 e do Prov. CNJ 213/2026:
   análise prévia de risco (art. 7º I), avaliação de impacto no tratamento de dados (7º II),
   checklist das 5 cláusulas contratuais mínimas (art. 8º), ficha de comunicação anual à Corregedoria
   (6º V e 12), política de registro interno de usos para auditoria (6º VI), roteiro da capacitação
   obrigatória com os 5 conteúdos do art. 11 V. **Nenhum player vende isso**, e há **prazo legal
   correndo** com sanção que chega a falta grave. O parente mais próximo na família é o `etica-adv-os`.
2. ⭐ **Defesa técnica do titular** — PAD, responsabilidade civil do art. 22, memória de fundamentação
   da recusa/exigência. **Nenhum ERP e nenhuma entidade de classe vende ao titular a peça com que ele
   se defende.** É a postura do `etica-adv-os` transposta para a delegação.
3. ⭐ **Varredura de vigência do CNN** — o AryaBolt promete "atualizações de legislação aplicadas
   instantaneamente" como feature de assinatura, mas **nenhum deles publica COMO verifica** se um
   provimento foi absorvido, é autônomo ou está suspenso.

**Sete frestas adicionais que F1-F4 provam e F5 não viu** — todas cabem no art. 5º do Prov. TJMT
(organizar, sumarizar, preparar minuta preliminar, automatizar rotina), nenhuma no art. 4º:

4. ⭐ **As obrigações periódicas auditáveis.** Remessa quinzenal ao **RCTO** e à **CESDI** nos dias 5
   e 20, **inclusive negativa** (CNN 267 e 270), e sincronização quinzenal do **CCN/Índice Único**
   (CNN 311). "Nenhuma ferramenta de gestão que encontrei nesta pesquisa cobre a rotina quinzenal com
   informação negativa" — F2 §6, T-62. É calendário, não redação, e é o que aparece em correição.
5. ⭐ **A cláusula de meios e formas de pagamento (CNN 165-A).** Obrigação de 2024, cinco incisos,
   regra própria para terceiro pagador e para a recusa da parte, **e ninguém automatizou**. F2 §12.5:
   "é pequena, determinística e cara de errar" — o produto de escritura mais defensável.
6. ⭐ **A ata de arrematação hipotecária.** Título translativo, competência própria, conteúdo mínimo
   na lei e **zero regulamentação do CNJ** — o perfil de ato em que o delegatário mais se expõe
   (F3 §7.4).
7. ⭐ **O relógio dos 15 dias da cessão de precatório** (F3 §6.2) — "não é controlado por nenhuma
   ferramenta de gestão de serventia encontrada".
8. ⭐ **O termo de recusa fundamentada** — lacuna normativa federal que vira produto: prova
   constituída de que o titular qualificou e decidiu (F2 §8, F4 §5.4).
9. ⭐ **O checklist de pré-correição anual** (CNN 105) — a correição é **anual e previsível**, o que a
   torna "o melhor produto preventivo possível" (F4 §5.3).
10. ⭐ **O algoritmo de competência do ato eletrônico** — 4 passos, determinístico e auditável,
    "exatamente o tipo de coisa que um plugin resolve melhor que um manual" (F2 §7, T-26).

### 6.4 A leitura de posicionamento

O eixo do produto **não pode ser "redigir a minuta"** — ali o concorrente é o CNB, dentro da
plataforma do CNB, provavelmente de graça. O eixo defensável é o que o titular **não consegue
comprar de ninguém**: a **conformidade**, a **defesa**, a **vigência** e o **calendário**. É o mesmo
movimento que a família já fez no `etica-adv-os` (defender o próprio profissional) e no
`holding-architect` (vender a verdade dura em vez da promessa fácil).

---

## 7. Mercado e preço

### 7.1 Os números, com selo

| Indicador | Valor | Selo | Fonte |
|---|---|---|---|
| Serventias extrajudiciais no país | **12.210**, em 5.569 municípios | ✅ | CEN 7ª ed. 2025, cap. Capilaridade, fonte declarada CNJ/Painel de Dados |
| Corroboração interna do 12.210 | 6.193 homens + 5.950 mulheres + 67 não declarados = **12.210** titulares, via **Justiça Aberta/CNJ** | ✅ | CEN 7ª ed., cap. Igualdade de Gênero |
| Contagem alternativa **na mesma edição** | "mais de **12.512** unidades extrajudiciais" (cap. Desjudicialização) | 🟡 **inconsistência interna declarada da Anoreg** | CEN 7ª ed. |
| O "~13.440" da meta-pesquisa | **Não se confirma** na edição corrente | — | F5 |
| **Serventias com atribuição de Notas** | **8.228 — 67,4%, a maior atribuição do país** | ✅ | CEN 7ª ed. |
| Demais atribuições | RCPN 7.201 · Protesto 3.846 · RTD/RCPJ 3.810 · RI 3.682 · RCM 556 · RD 347 (soma 27.670 — serventia acumula atribuições) | ✅ | CEN 7ª ed. |
| Emprego direto no setor | **96.740** (95.099 CLT + 1.641 estatutários) | ✅ | CEN 7ª ed., fonte CNJ |
| Atribuição mais procurada pelo cidadão | **Notas — 38%** (Registro Civil 30%, RI 18%, Protesto 12%, RTD 12%, Ofício Único 8%, RD 3%) | ✅ | Datafolha 2025, via CEN 7ª ed. |
| Procurações públicas 2007 → 30/11/2025 | **55 milhões** | ✅ | CEN 7ª ed. |
| Atos no e-Notariado (acumulado) | **9 milhões** — 2,3 mi escrituras · 584 mil procurações · 1,8 mi e-Not Assina · 2,5 mi certidões eletrônicas · **17 mil atas notariais** · 55 mil AEVs · 15 mil AEDOs | ✅ | CEN 7ª ed. |
| Inventários / divórcios extrajudiciais desde 2007 | **+2,3 mi** / **+1 mi** de atos | ✅ | CEN 7ª ed. |
| Faturamento — a moda | **4.032 serventias (32,1%) na faixa R$ 10.001-50.000 brutos/mês** | ✅ (quantidades) | CEN 7ª ed., cap. Faturamento |
| Faturamento — capacidade de compra | **8.139 serventias (64,9%) acima de R$ 10 mil brutos/mês**; **4.107 (32,7%) acima de R$ 50 mil** | ✅ quantidades / 🟡 percentuais recalculados por F5 | CEN 7ª ed. |
| Faturamento — quem não compra | **2.998 serventias (23,9%) com até R$ 5 mil brutos/mês** | ✅ | CEN 7ª ed. |
| ⚠️ Honestidade sobre o dado | A **coluna de percentual publicada não reconcilia** com as quantidades (soma 95,1%). F5 usou as **quantidades**, internamente consistentes, e recalculou os percentuais | 🟡 declarado | F5 |
| Bruto ≠ líquido | Repasses legais variam por UF de **~5% a ~39%** do arrecadado, mais **35,09%** de despesas de funcionamento (🟡 média setorial de estudo encomendado, não auditoria), mais IR e ISS. Regra de bolso: **R$ 50 mil brutos ≈ R$ 20-25 mil líquidos antes do IR** | ✅ (a variação por UF) / 🟡 (o 35,09%) | CEN 7ª ed., 27 pp. |
| 🔴 Aberto | **Distribuição por UF** da atribuição de Notas, e validação real de faturamento — existem no **Painel de Dados Estatísticos das Serventias Extrajudiciais (Justiça Aberta/CNJ)**, que exporta `.csv`/`.xlsx` por serventia com produtividade e receita. **É consulta ao painel, não pesquisa web** | 🔴 | F5 |

### 7.2 O universo endereçável

**8.228** serventias com atribuição de Notas. Aplicando o corte de capacidade de pagamento:

- corte >R$ 10 mil brutos/mês (64,9%) → **~5.300 serventias** 🟡 (derivação de F5)
- corte conservador >R$ 50 mil/mês (32,7%) → **~2.700 serventias** 🟡

**O comprador é único e sem comitê** — Lei 8.935/94, art. 21: o gerenciamento administrativo e
financeiro é de responsabilidade **exclusiva do titular**, inclusive investimento e pessoal. Um "sim"
fecha a venda. É melhor que o advogado de escritório. ✅ **Exceção:** serventia **vaga** (interino)
precisa de **autorização prévia da Corregedoria**, com "valor compatível com o mercado" (Prov. TJMT
1/2026, art. 9º) — nesse segmento, preço fora de curva trava a compra por via administrativa.

### 7.3 As âncoras de preço que existem

| Âncora | Valor | Direção da ancoragem |
|---|---|---|
| AryaBolt, plano de entrada | **R$ 449/mês = R$ 5.388/ano** | O piso do que um titular **já aceita pagar** por software com IA |
| AryaBolt, "Mais Recomendado" | R$ 949/mês = R$ 11.388/ano | Ponto médio declarado do mercado |
| AryaBolt, Premium | R$ 1.349/mês = R$ 16.188/ano | Teto público |
| **@Bolt isolado (IA de redação)** | R$ 49/mês + tokens | ⚠️ Ancoragem **para baixo** — existe IA notarial a R$ 588/ano |
| **IA Not (CNB/CF)** | 🟡 sem preço anunciado, provavelmente embutido | ⚠️ Ancoragem **para zero** no caso de uso "propor minuta" |
| Família IA Combativa, tier flagship | R$ 498 pagamento único | civel, criminal, franchising, holding, eleitoral |

### 7.4 ✅ FECHADO — R$ 498, pagamento único (P-2)

**Decisão cravada do Doc:** **R$ 498, pagamento único**, com a política de **"atualizações
exclusivas para membros da comunidade IA Combativa"** promovida a **argumento central da oferta** —
não nota de rodapé. É a mesma política que a família adota desde o `direito-familia`; aqui ela muda
de status, porque é ela que sustenta a promessa ao longo do tempo (§7.6).

O raciocínio da F5 que sustenta o número, integralmente:

**Por que 498 e não menos** — é **1,1 mês do plano de entrada do concorrente, pago uma vez**, e a
ancoragem escreve sozinha ("o que o mercado cobra por mês, aqui você paga uma vez"); a capacidade de
pagamento está provada por dado (65% acima de R$ 10 mil brutos/mês, moda na faixa R$ 10-50 mil); o
produto entrega uma camada que **nenhum concorrente vende** — os artefatos de conformidade do Prov.
1/2026, **com prazo legal correndo** e sanção que chega a falta grave, e necessidade com prazo tem
elasticidade baixa; e o comprador é titular de delegação, o perfil que a família já precifica no topo.

**Por que não acima de 498** (a tentação, dado o AryaBolt a R$ 16 mil/ano) — é o **primeiro plugin da
família vendido a um delegatário de serviço público**, e a intuição dos 35 anteriores não transfere;
passar do teto histórico num comprador novo **mistura duas variáveis num teste só** (se não vender,
não se sabe se foi o preço ou o comprador); e o art. 9º do Prov. TJMT trava por "valor compatível com
o mercado" na fatia de serventias vagas.

**A alternativa que foi descartada** — R$ 398 ampliaria o alcance para a faixa R$ 5-10 mil/mês (mais
1.411 serventias, 11,2%) e alinharia com `direito-imobiliario` e `agrario`. Registrado para
rastreabilidade; o Doc escolheu 498.

**E o piso que a pesquisa já excluía** — abaixo de 398 não se sustenta: o `calculosjudiciais` a
R$ 98,80 funciona porque a dor é universal; aqui a base endereçável é **~5.300**, não 1,4 milhão de
advogados. **Preço baixo em base pequena não compra volume, só destrói margem.**

### 7.5 O alerta que F5 diz valer mais que o número

**Este é o plugin da família em que o pagamento único envelhece mais rápido.** A norma operacional
muda ~2× por mês (57 alterações do CNN em 24 meses, 16 só em 2026); o Prov. CNJ 213/2026 revogou o
74/2018 e foi alterado **5 meses depois** pelo 243/2026; a tabela do RJ teve **duas vigências dentro
de 2026**. Um comprador que pague hoje por "a norma vigente" tem, em doze meses, um produto que
**cita norma revogada** — exatamente a falha que o produto se vende para evitar. O concorrente
resolve isso estruturalmente: assinatura, com "alterações de legislação aplicadas instantaneamente".

F5 registrou que **é a primeira vez que a família encontra um domínio que pediria assinatura por
natureza da norma, não por preferência comercial** (§6.4). **O Doc escolheu pagamento único (P-2)** —
o que não elimina o problema, transfere-o para a arquitetura. É o que a §7.6 fecha.

### 7.6 ⭐ O que a arquitetura PRECISA ter para o pagamento único não virar promessa falsa

Com P-2 cravado, o alerta da F5 deixa de ser ressalva comercial e vira **requisito de produto**. O
risco é nomeável: *um comprador que pague R$ 498 hoje por "a norma vigente" tem, em doze meses, um
produto que cita norma revogada — exatamente a falha que o produto se vende para evitar.* Três
requisitos, todos derivados de achados das frentes, não de preferência:

**R-A · Data de corte explícita, em todo artefato de norma.** Nenhuma saída do plugin afirma
vigência sem dizer **de quando** é a sua base. É o padrão `context/travas-defasagem.md` que a família
já usa, aqui elevado a condição de honestidade da oferta.

**R-B · O PDF compilado oficial do CNN, versionado como artefato único.** Ele existe e está
identificado: **369 páginas, consolidado até o Provimento 253/2026**, baixado pela F2 (§12.3 ✅). A
meta já recomendava "um arquivo único versionado com data de corte" — agora ele tem nome, tamanho e
número de corte. Não é uma lista de provimentos soltos; é **um documento** que se troca inteiro
quando envelhece.

**R-C · Rotina de refresh de DOIS canais — e é aqui que a maioria das ferramentas erraria.** A F1
provou que vigiar só o CNN **não basta**: o **Provimento 247/2026 (VNS)** não alterou o Código — é
**autônomo** —, criou cobrança por ato (R$ 1 / R$ 10 / R$ 25 por faixa de emolumentos) e foi
**suspenso em menos de uma semana**. *"Uma rotina que só vigie o CNN não veria isso."* (F1 §0.5 ✅).
Logo, os dois canais são:

| Canal | O que vigiar | Como se detecta | Cadência justificada |
|---|---|---|---|
| **① O CNN** | Ficha do Prov. 149/2023 — campos `Alteração` e `Situação`; e o texto compilado quando a ficha mudar | Novo provimento no fim da lista; ou marcação `(suspenso …)` nova | **Quinzenal** — 57 alterações em 24 meses, **16 só em 2026** ≈ **2 por mês** |
| **② Provimentos autônomos da Corregedoria — os que NÃO alteram o CNN** | Varredura sequencial da base de atos a partir do último id conhecido (**6998 = 24/08/2026**), lendo `Origem: Corregedoria` | Qualquer provimento com número **> 255** | **Quinzenal** — é o canal que pega o 247/2026 |

E os **quatro campos** que o `context/` precisa guardar para que uma skill de gate consiga comparar
(F1 §7): **data de corte · número do último provimento alterador (hoje 253) · último id varrido na
base do CNJ (hoje 6998) · lista de suspensos ativos com data-limite** (hoje: 172, 175 e 247 — este
com prazo vencendo por volta de **12/10/2026**).

**Como isso fecha com a política da comunidade (P-2):** o pagamento único compra o produto; a
comunidade compra **a continuidade dos quatro campos acima**. Essa é a linha que torna a política um
argumento central honesto em vez de um upsell — o comprador pontual recebe a versão estável com data
de corte declarada, e sabe exatamente o que envelhece e quando.

---

## 8. Os 🔴 abertos — consolidado

Tudo o que nenhuma frente fechou, com o que **exatamente** falta e se **bloqueia ou não** o build.
"Bloqueia" significa: sem isso, uma skill nasceria afirmando o que não se sabe.

### 8.1 Bloqueiam uma skill específica (não o produto)

| # | O que ficou aberto | O que falta para fechar | Bloqueia |
|---|---|---|---|
| A-01 | **Procedimento de recusa/exigência do tabelião de notas** — não há norma nacional; é código estadual, 27 fontes | Varredura dos códigos de normas estaduais, ou decisão de escopo (ver D-5) | **Sim, a skill de exigência** — F2 §11.1: "pesquisa dedicada obrigatória antes de construir a skill" |
| A-02 | **Íntegra do Provimento CSM 2.753/2024 (TJ/SP)** sobre cessão de precatório — `notariado.org.br` e `cnbsp.org.br` responderam **403** | Buscar no **DJE do TJ/SP** ou nas NSCGJ-SP consolidadas; e checar se há ato posterior de 2025 | **Sim, a skill de cessão de precatório com cobertura de SP** (o maior mercado) |
| A-03 | **Competência do ato notarial HÍBRIDO** (CNN 313) — o texto autoriza, mas não diz se seguem os arts. 302-304 ou o art. 8º | Pesquisa dedicada, ou declarar a lacuna na própria skill | **Não bloqueia** — mas é pergunta que o usuário faz na primeira semana; a skill **tem de declarar a lacuna** em vez de escolher |
| A-04 | **Regulamentação estadual da arbitragem notarial** — a varredura de F3 foi federal | Varredura por CGJ antes de escrever a skill de arbitragem | **Sim, a skill de arbitragem** (que já nasce com aviso 🔴 de ausência de rito nacional) |
| A-05 | **Existência da "central notarial de âmbito nacional"** do art. 6º-A §2º, que é a condição de operação do acesso dos tabeliães aos dados dos tribunais | Consultar o CNB/CF. Sem ela, o §2º é letra morta na prática | **Parcial** — a skill de precatório precisa saber se o canal existe |
| A-06 | **Subseção VI do Cap. VI do CNN** (entre os arts. 299 e 312) — a varredura estrutural não encontrou o cabeçalho | Leitura linear de `capturas/cnn-05-…` entre os arts. 299 e 312 | **Não** — mas o índice de endereçamento fica com um buraco |
| A-07 | **Anexos do CNN** — o Prov. 253 altera o "item 1.4.4 do **Anexo VIII**"; os anexos não foram inventariados | Mapear os anexos (vários carregam **modelos operacionais**) | **Não bloqueia, mas é conteúdo perdido** |
| A-08 | **Ementa específica dos Prov. 173, 181 e 190** (ementas oficiais genéricas) e **se o Prov. 219/2026 realmente altera o CNN** | Ler o texto de cada um (`detalhar/5615`, `/5729`, `/6088`, `/6806`) e mapear artigo a artigo | **Não** |
| A-09 | **Vedação sucessória específica de testemunhas** (herdeiro, legatário, beneficiado) — o artigo exato da parte de sucessões não foi capturado | Captura do CC, parte de sucessões | **Não** — a skill de testamento cita o CC 228 e marca a doutrina como doutrina |
| A-10 | **Substabelecimento particular** de mandato público quando o ato-fim exige forma pública (CC 655 × 657) | Jurisprudência dirimente | **Não** — declarar a divergência |
| A-11 | **Súmula 377/STF** e o estado atual da comunicação de aquestos na separação obrigatória — impacta a exigência (ou dispensa) de **outorga conjugal** | Pesquisa dedicada | **Não** — o plugin marca divergência (T-44) |
| A-12 | **CNDT (débitos trabalhistas)** — há indício de que o CNJ tratou CND/CPEN e CNDT de modo **diferente**. `cnbsp.org.br` bloqueou o acesso (403) | Ler a decisão | **Não** — a skill **não mistura** os dois (T-38b) |
| A-13 | **"30 salários mínimos" do CC 108** — base de medida (valor do negócio × venal × base do ITBI) | Fonte primária dirimente | **Não** — declarar a divergência |
| A-14 | **CAR e georreferenciamento na escritura comum de imóvel rural** — a norma lida (CNN 416) é do procedimento de **usucapião**; a extensão à escritura ordinária é prática, não texto | Norma nacional expressa, se existir | **Não** — marcar 🟡 |
| A-15 | **LC 227/2026 (ITCMD) e LC 214/2025 (IBS/CBS)** — impacto na **escritura** não pesquisado (F3 cobriu o ITCMD na desjudicialização, não na compra e venda) | Frente dedicada | **Parcial** — a skill de escritura não afirma nada sobre eles |
| A-16 | **REsp 2.115.909/SP** (e-mail não é testamento) e o **REsp-âncora sobre print de WhatsApp sem hash/ata** | Conferência no `scon.stj.jus.br` | **Não** — os dois estão 🟡 e não podem virar afirmação |

### 8.2 Não bloqueiam o build — viram rotina de vigilância

| # | Item | O que fazer |
|---|---|---|
| B-01 | **STF, MS 40.223** (AF por instrumento particular) — julgamento presencial pendente, pode derrubar o art. 440-AO do Prov. 246/2026 | **Postura honesta:** a regra vigente é a do Prov. 246, **e o STF pode mudá-la**. Vigiar mensalmente até o julgamento (F1, R7) |
| B-02 | **ADI, liminar ou precedente vinculante contra a Res. CNJ 571/2024** — nenhum encontrado. **Não é prova de ausência** | Checagem periódica no STF e no CNJ — item de rotina, não fato fechado (F3) |
| B-03 | **Decisão que suspendeu o Prov. 247/2026** (VNS) — número do processo e ato formal; a data 13.8.2026 e o prazo de 60 dias vêm de fontes setoriais | Vigiar o fim dos 60 dias — **marcar ~12/10/2026** (F1, R4) |
| B-04 | **Data da liminar que suspendeu 172/175** — fontes secundárias divergem (27 × 28/11/2024) | **Não citar a data**; citar a suspensão e o desfecho de 24.7.2026 |
| B-05 | **Precedente específico do STF sobre competência concorrente do CNJ** e o **Tema 940** (dupla garantia) — não abertos | Ancorar na **letra** do art. 103-B §4º III, que é fonte primária e basta (F4) |
| B-06 | **Acórdãos da controvérsia de legitimidade passiva pós-Tema 777** — artigo da ConJur retornou 403 | Tratar como **controvérsia noticiada**, nunca como certeza (T-98) |
| B-07 | **Jurisprudência em Teses do STJ, ed. 229** — existe na base, o texto não abriu | Ler antes de citar qualquer tese |
| B-08 | **Ausência de súmula/repetitivo do STJ** sobre responsabilidade notarial | Registrar como **ausência declarada**, não como prova de inexistência (T-109) |
| B-09 | **Se a Res. CNJ 303/2019 impõe dever direto ao tabelião** — lida em resultado de busca, não em captura verbatim | Capturar `atos.cnj.jus.br/atos/detalhar/3130` |
| B-10 | **Conteúdo dos 57 provimentos alteradores** — foi lido o texto consolidado com marcadores, não cada ato | Checar situação **ato a ato** antes de citar; e ver **D-1** da §4.1 (divergência de método entre F1 e F3) |
| B-11 | **Tração real do AryaBolt** ("3.516 cartórios") | Se o Doc quiser dimensionar a ameaça, **falar com 2-3 titulares** — não pesquisar mais |
| B-12 | **Preço e modelo de cobrança da IA Not** — nenhuma fonte pública anuncia | Se for gratuita dentro do e-Notariado, a fresta "propor minuta" é ainda menor |

### 8.3 Não bloqueiam o build — são decisão de escopo, não pendência de pesquisa

| # | Item | Por que é decisão, não pesquisa |
|---|---|---|
| C-01 | **Códigos de normas estaduais dos 27 TJs** — cada TJ mantém o seu, e o CNN **não os substitui**; convive com eles | É "mais uma frente inteira" (F1, R8). Ver **D-3** |
| C-02 | **Rito e prazo prescricional do PAD nas 26 UFs restantes** — só o caso do RJ foi visto, e por reportagem | F4 formula a decisão nestes termos: *"o plugin cobre a estrutura federal + 'confira seu estado', ou nasce com N tabelas estaduais?"* Ver **D-3** |
| C-03 | **Quantas UFs além de MT já regularam IA em serventia** | "É o `context/` que mais vai envelhecer" (F5). Ver **D-3** |
| C-04 | **Distribuição por UF da atribuição de Notas + faturamento real por serventia** | Existe no **Painel Justiça Aberta/CNJ** (`.csv`/`.xlsx`) — é **consulta ao painel**, não pesquisa web. Só necessário se houver campanha regionalizada. Ver **D-2** |
| C-05 | **Apetite real de preço** | Nenhuma pesquisa substitui **falar com 2-3 titulares**. A faixa de F5 é derivada de âncora de concorrente e capacidade de pagamento, **não de conversa com comprador**. Ver **D-1** |

---

## 9. O QUE CONTINUA SENDO DECISÃO DO DOC

Os três botões de 25/08/2026 (**P-1** conformidade de IA como diferencial central · **P-2** R$ 498
pagamento único com a comunidade como argumento central · **P-3** nome `tabelionato-os`, v0.1 =
Notas isolado) **saíram desta seção** e estão na §0 como premissa. O que segue é só o que as cinco
frentes deixaram genuinamente aberto — e nenhuma destas é pergunta que mais pesquisa resolve: **as
três primeiras exigem ação humana fora da web**, e as duas últimas são escolha de escopo.

---

### D-1 · Falar com 2-3 titulares — validação de apetite (ação humana, não pesquisa)

**O 🔴 que nenhuma frente fecha, e as duas que tentaram dizem a mesma coisa.** A meta recomendou
"testar preço com 2-3 titulares reais antes de fixar a Kirvano"; a F5 fechou a faixa **derivada de
âncora de concorrente e capacidade de pagamento — não de conversa com comprador** (§8.5 🔴).

Com **P-2 cravado (R$ 498)**, a pergunta muda de "quanto cobrar" para **"o que a conversa ainda
altera"**. Três coisas que só um titular real responde, e nenhuma delas é o preço:

1. **O eixo escolhido ressoa?** P-1 aposta que conformidade de IA + defesa vale mais que redação de
   minuta. Isso é uma **hipótese de dor**, não um fato — a pesquisa provou que o espaço está livre,
   não que o titular sente falta dele.
2. **Ele já ouviu falar da IA Not?** Se o CNB entregou bem, a percepção de "IA de cartório = grátis,
   já vem no e-Notariado" é uma objeção de venda que a copy precisa responder de saída.
3. **A ancoragem funciona?** *"O que o mercado cobra por mês, aqui você paga uma vez"* depende de o
   titular conhecer o preço do AryaBolt. Se não conhecer, a âncora não ancora nada.

| Opção | Consequência |
|---|---|
| **(A) Conversar antes do build** | Corrige o eixo enquanto corrigir ainda é barato. Custo: atrasa o início |
| **(B) Conversar entre o build e o lançamento** | Não atrasa a construção, e ainda dá tempo de reposicionar copy, capa e divulgação. **Não** dá tempo de mudar a arquitetura de camadas |
| **(C) Lançar e aprender pela venda** | É o padrão da família nos 35 plugins anteriores. **Aqui o risco é maior:** é o primeiro comprador delegatário, e a F5 avisa que a intuição dos anteriores não transfere |

---

### D-2 · Consulta ao painel Justiça Aberta / CNJ (ação humana, não pesquisa web)

**O que existe lá e não existe em lugar nenhum:** o **Painel de Dados Estatísticos das Serventias
Extrajudiciais** exporta `.csv`/`.xlsx` **por serventia**, com **produtividade e receita**. A F5 não
extraiu porque é **dashboard dinâmico, não página estática** — e diz literalmente: *"é uma consulta
ao painel, não uma pesquisa web"* (§8.1 🔴).

**O que isso destrava:** (a) a **distribuição por UF** da atribuição de Notas — a 7ª edição do
Cartório em Números só publica o total nacional (8.228); (b) a **validação real de faturamento**,
hoje dependente da amostra da Anoreg, cuja **coluna de percentuais não reconcilia** com as
quantidades (§7.1 🟡).

| Opção | Consequência |
|---|---|
| **(A) Consultar agora** | Permite campanha regionalizada e substitui uma amostra 🟡 por dado ✅. Custo: uma sessão manual no painel |
| **(B) Consultar só se houver campanha por UF** | O número nacional (8.228 ✅) já basta para decidir e para a copy. O recorte por UF só importa quando houver segmentação de mídia |
| **(C) Não consultar** | Mantém o dimensionamento no que a Anoreg publica — que é ✅ no total e 🟡 no faturamento, com inconsistência interna declarada |

---

### D-3 · Varredura das 27 corregedorias (ação humana; e é a que mais envelhece)

Quatro camadas do produto dependem de norma estadual — e **três delas não são periféricas**:

| Camada | O que falta | Frente |
|---|---|---|
| **Normas estaduais de IA em serventia** | Quantas UFs além de MT já regularam. A F5 achou MT como a primeira e uma indicação 🟡 (Anoreg/RS) de que outras corregedorias "passaram a discutir" | F5 §8.4 🔴 |
| **Rito e prazo prescricional do PAD** | Só o caso do RJ foi visto (DL estadual 220/1975, 2 anos), e **por reportagem do STJ**. Os outros 26 não foram levantados | F4 §9.5 🔴 |
| **Procedimento de recusa/exigência do tabelião de notas** | **Não existe equivalente federal.** O instrumento é estadual | F2 §11.1 🔴 |
| **Emolumentos** | A F5 verificou SP, RJ, MG, RS e DF; as outras 22 não | F5 §1.3 |

**Com P-1 cravado, esta decisão ficou mais pesada do que era.** A camada de conformidade é o
diferencial central, e ela é justamente a que a F5 aponta como *"o `context/` que mais vai
envelhecer"*.

| Opção | Consequência |
|---|---|
| **(A) Só a estrutura federal + "confira seu estado"** (padrão que a família já usa em emolumentos e no rol da ANS) | Nasce agora, com o corpus já capturado. **Mas** a promessa fica limitada exatamente onde o titular mais precisa: como recusar, quanto cobrar, qual o prazo da defesa dele — e, com P-1, se ele pode usar IA |
| **(B) Varrer as 27 antes de lançar** | Cobertura real. Custo: **uma frente inteira por bloco de camadas** — F1 R8, F2 §11.1, F3 §12.6 e F4 §9.5 dizem isso, cada uma para a sua camada |
| **(C) Federal no v0.1 + varredura como entrega da comunidade** | Casa com P-2: o pagamento único compra a estrutura federal; a comunidade recebe as UFs conforme entram. Começar pelas que a F5 já verificou (SP, RJ, MG, RS, DF) e por **MT**, que é a única com norma de IA |

---

### D-4 · A ponta registral fica dentro do v0.1 como contexto, ou fora?

**P-3 fechou o recorte** (Notas isolado; RI vira irmão ou v0.2). Sobra uma pergunta que P-3 não
responde e que as frentes deixaram explícita: **três institutos têm ponta notarial e ponta
registral**, e o tabelião tem **dever expresso de orientar** sobre a inviabilidade da via
extrajudicial (CNN 440-G §1º ✅ F3).

| Instituto | Ponta notarial (dentro do v0.1) | Ponta registral |
|---|---|---|
| Usucapião extrajudicial | A ata do inciso I (competência **vinculada**) | Todo o processo — notificações, edital, ciência aos entes, decisão, registro |
| Adjudicação compulsória | A ata (livre escolha, salvo diligência) | Protocolo, **notificação do requerido**, impugnação, recurso, registro |
| Execução extrajudicial de hipoteca | **A ata de arrematação** — e ela é **título translativo** | Intimação para purgar mora, averbação da excussão, registro da ata |

| Opção | Consequência |
|---|---|
| **(A) Contexto de orientação, sem skill de execução** | O plugin explica o que vem depois para que o titular oriente — cumprindo o dever do 440-G §1º — mas nunca executa ato do registrador. É o menor escopo que ainda honra o dever legal |
| **(B) Nem contexto — declarar a fronteira e parar na ata** | Escopo mínimo. **Risco:** o titular fica sem base para orientar sobre inviabilidade, que é dever expresso dele |
| **(C) Contexto + cross-link com o futuro plugin-irmão de RI** | Padrão que a família já usa (`execucao` × `juris` × `calculosjudiciais`). Só funciona quando o irmão existir |

---

### D-5 · A rotina de refresh — quem opera

**A §7.6 fixou O QUE vigiar** (dois canais, quatro campos, cadência quinzenal justificada por dado).
Falta decidir **quem opera** — e isso é custo recorrente, não desenho.

| Opção | Consequência |
|---|---|
| **(A) Rotina manual do Doc, quinzenal** | Zero infraestrutura. Custo: duas varreduras quinzenais recorrentes (ficha do CNN + ids novos na base do CNJ), indefinidamente |
| **(B) Script + agendamento** que compara os quatro campos do `context/` e avisa quando algo muda | É o desenho que a F1 §7 já especificou (R1-R8). Custo: mais um artefato para construir e manter; a base do CNJ é HTML, não API |
| **(C) Não fazer, e assumir a defasagem** | Aceitável em outros plugins da família (norma anual). **Aqui não:** com P-2 (pagamento único) e a promessa de "norma vigente", não vigiar transforma o produto na falha que ele se vende para evitar |

---

*Consolidação escrita em 25/08/2026 a partir das 5 frentes de pesquisa dedicada, revisada no mesmo
dia para incorporar os três botões do Doc (§0) e a **revisão 2 da F4**. Nenhum DESIGN-SPEC, PRD ou
build foi criado a partir deste documento — é o insumo da decisão, não a decisão. Arquivo:
`_planning/novas-verticais/tabelionato/DOSSIE-CONSOLIDADO.md`.*

---

## Adendo obrigatório — varredura estadual e frentes F6-F9

Este adendo integra as travas posteriores ao dossiê-base e prevalece em divergências sobre as 27 UFs.

### A régua dos cinco falsos positivos de IA

“O tribunal usa IA nos próprios processos” não significa “a norma regula o uso de IA pelo delegatário”. Antes de classificar, conferir: **destinatário**, **veículo/autoridade** e **objeto**.

| UF/ato que parece norma de IA | Por que não vincula a serventia |
|---|---|
| ES — Prov. 21/2019, Centro de IA da CGJ | estrutura interna da Corregedoria para seus processos |
| BA — Decreto Judiciário 1007/2025, Comitê de IA do TJBA | governança interna para magistrados e servidores |
| CE — Portaria Conjunta 03/2026/PRES/CGJCE, tradução com IA | ferramenta do contexto judicial 🟡 |
| PI — Prov. 151/2023, critério de vitaliciamento | código judicial e avaliação de magistrado; o extrajudicial está no Prov. CFE 62/2024 |
| AM — Resolução TJAM 29/2026 | ato do Tribunal Pleno para o próprio TJAM, ancorado na Res. CNJ 615/2025 |

Vizinhos de IA — TI, segurança, proteção de dados e automação — podem vincular sem regular IA: DF art. 175, VII; SP Prov. 16/2025 e Cap. XIII, Seção VIII; PE Cap. VI; AL Tít. VIII; PI Tít. I, Cap. VII; RN arts. 60-A a 60-Q; RS Prov. 19/2026; AP Prov. 0514/2026.

### Remissões mortas em norma viva

- **MT:** Prov. 1/2026 cita o revogado Prov. CNJ 74/2018; remeter materialmente ao Prov. 213/2026 e alterações, com nota sobre a desatualização estadual.
- **MS:** cinco remissões ao Prov. 74/2018 e nenhuma ao 213/2026.
- **SE:** art. 62, V ainda cita a Lei 6.310/2007 superada.
- **RN:** LC 165/1999 foi revogada pela LC 643/2018.
- **MG:** Prov. 260/2013 foi superado.
- **DF:** Provimento-Geral de 2013 foi integralmente revogado em abril de 2026.
- **MA:** Título III do Prov. 16/2022 foi revogado.
- **CE:** arts. 93-107 foram revogados e o rito migrou à Resolução 03/2020.

A marcação é por **dispositivo**, não apenas por diploma. O estado “suspenso” também é autônomo: Provimentos CNJ 172, 175 e 247; em RR, a Lei 1.157/2016 está suspensa e continua aplicável a Lei 752/2009.

### Os dois relógios

| Relógio | Prazo | Início e trava |
|---|---|---|
| PAD | estadual: 17 UFs com prazo, 9 ausências/remissões insuficientes e RO como lacuna | conhecimento/ciência ou data do fato/evento conforme a UF; não presumir Lei 8.112/1990; no PI, LC 234/2018, art. 40, §§1º e 3º |
| civil, art. 22 | triênio somente desde 11/05/2016 | letra: lavratura; STJ: trânsito em julgado da anulatória quando o dano só nasce ali, REsp 2.043.325 |

Testamento evidencia a actio nata: guarda permanente e eficácia após o falecimento podem ocorrer décadas depois da lavratura.

### Livro não se elimina porque foi digitalizado

Todos os livros de Notas têm guarda permanente pela Tabela de Temporalidade do Provimento CNJ 50/2015, classe 3-5-1, cuja adoção é obrigatória pelo CNN art. 196. A digitalização pode permitir eliminar **documentos instrutórios**, nunca o livro, e só com o rito do CNN arts. 92-93, desfiguração, comunicação semestral e ressalva de valor histórico do Decreto 10.278/2020. O índice e metadados derivados continuam sendo tratamento de dados pessoais sob a LGPD.

### Estados, endereços e destinatários

- CNN: 57 alterações; última 253/2026. O Prov. 244/2026 não alterou o Código; o alterador de 21/07 foi o 242; 228 e 229 existem ambos.
- O CNJ empilha versões; vence a última redação por data. Exposição de Motivos e página de listagem não provam vigência.
- Arbitragem e precatório têm zero ocorrência no CNN; remissões nominais do Código, como art. 441, II ao Prov. 56/2016, continuam relevantes enquanto vigentes.
- Art. 216-B da LRP veio da Lei 14.382/2022; o art. 7º-A inteiro veio da Lei 14.711/2023; 6º-A é precatório e 7º-A reúne condição negocial, mediação/conciliação, arbitragem e conta vinculada.
- §7º do art. 7º foi vetado, embora o art. 7º-A, §3º remeta a ele; §§3º e 4º do art. 39 também foram vetados.
- SC art. 112 da LC 339/2006 é de magistrado; PR art. 765 é Protesto; CE art. 172 fala em registrador; Res. 615/2025 não vincula diretamente a serventia; a solidariedade do ITR nomina o Registro de Imóveis.

### Fontes oficiais que enganam sem controle de vigência

- Página desatualizada: PE, SE, MG e CE. Apontar para o ato, não para a listagem.
- Notícia institucional não fecha bloco: MG chamou alteração de “novo Código”; fonte atribuída ao PR continha notícia falsa; no AM, matérias do mesmo domínio divergiam.
- Consolidado não equivale a vigente: ES versão 6.2 omite três atos posteriores; RN para em 05/12/2023; PR distingue “atualizado” de “compilado”.

### Citação que parece certa e leva ao dispositivo errado

- AL: número reinicia por Título — citar Título + artigo.
- SP: Tomo II começa no Capítulo XIII e usa itens, não artigos.
- GO: número sem ano é inválido para localizar com segurança.
- AP: manter quatro dígitos e zero inicial.
- TO: preservar a sigla variável da unidade emissora.
- RO e TO têm ato 21/2023 com objetos opostos.
- PB: sumário diverge do corpo; citar pelo corpo.
- RN: Código é Prov. 156/2016, não 154/2016.
- MT: “descreverá” no art. 18-H é erro do próprio documento; não corrigir silenciosamente em citação literal.

### Contagem de prazo

PR e MS usam dias úteis nas hipóteses mapeadas; SC e MT usam dias corridos nos procedimentos da serventia; SE usa dias contínuos. Uma regra única de contagem produz intempestividade.

### Acervo, IA e números que não podem ser inventados

- Autorização federal de IA no acervo: Prov. 213/2026, **Anexo II, item 3, VI**.
- Simulação de extração: bienal somente na Classe 3; 30 meses na Classe 2; 36 meses na Classe 1; imediata na troca de fornecedor.
- Logs: retenção de 5 anos. Retenção do **backup** não foi fixada 🔴.
- O Prov. 213 menciona IA uma vez para autorizar; vedações vêm das UFs.
- Acervo pertence ao serviço, não ao titular; deve ser transferido organizado ao sucessor.
- Vedação de treinamento alcança derivado — embedding, índice e sumário — quando contiver ou inferir dados protegidos.
- Não existe padrão nacional de nomenclatura de arquivo; existem requisitos de formato e metadados.

### Emolumentos

Percentual sobre o negócio é vedado; são 26 leis estaduais e uma federal para o DF. No DF, ato fora da tabela é gratuito. Vale a tabela temporalmente aplicável ao ato; erro do próprio serviço não gera cobrança. Nunca informar valor memorizado. A exceção supletiva de base identificada é a ata de usucapião do CNN art. 423, I, enquanto faltar lei estadual.

### Taxonomia estadual de recusa, exigência e dúvida

- **A1 (8):** PI, PA, TO, CE, MG, PB, RR, MA.
- **A2 (6):** AP, MS, RN, SC, RJ, ES.
- **A3 (3):** AL, DF, MT.
- **B (9):** AC, AM, BA, GO, PE, PR, RS, SE, SP.
- **C (1):** RO 🟡.

Não confundir: 17 UFs têm algum rito notarial; 8 têm prazo/nota dirigida ao tabelião; 6 fixam número de prazo. A dúvida alcança Notas em 14 UFs de modo geral; A3 é restrita ou remissiva.
