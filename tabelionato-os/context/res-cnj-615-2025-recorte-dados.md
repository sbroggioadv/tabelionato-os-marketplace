# Resolução CNJ n. 615, de 11/03/2025 — IA no Poder Judiciário · recorte DADOS, TREINAMENTO e ACERVO

> **Data de corte normativa: 25/08/2026.** Recorte dos arts. 19, § 3º, III, 26, § 4º, 27 e 30; conferir alterações posteriores antes do uso.

> **Fonte:** `atos.cnj.jus.br/atos/detalhar/6001` — extraído em **2026-08-25**.
> Publicada no **DJe/CNJ n. 54/2025, de 14/03/2025, p. 2-17**. Situação: **Alterada**
> (**Resolução n. 674, de 25/03/2026**). Substituiu a **Resolução CNJ n. 332/2020**.
> Comitê Nacional de IA do Judiciário designado pela **Portaria n. 270, de 27/08/2025**.
>
> ⚠️⚠️ **LEIA O ESCOPO ANTES DE CITAR.** Esta Resolução rege o **PODER JUDICIÁRIO** —
> tribunais, magistrados, servidores e colaboradores. **A serventia extrajudicial NÃO é órgão
> do Poder Judiciário**: é atividade privada em delegação (CF art. 236; Lei 8.935/94, art. 3º).
> Portanto a Res. 615/2025 **não se aplica diretamente ao cartório**. Ela chega ao foro
> extrajudicial **por remissão dos provimentos estaduais** — o Provimento TJMT/CGJ n. 1/2026 a
> invoca nominalmente nos consideranda ("CONSIDERANDO a obrigatoriedade de observância às
> diretrizes estabelecidas pela Resolução CNJ nº 615/2025"). Citá-la como se vinculasse a
> serventia por força própria é erro.
>
> ⚠️ **Recorte, não íntegra.** A Resolução tem **47 artigos + Anexo de Classificação de
> Riscos**. Abaixo estão os dispositivos de **dados, treinamento, armazenamento e
> auditabilidade** — os que tocam acervo. Extração de página web; confira na fonte.

---

## Fundamentos e curadoria de dados

**Art. 2º, IX** — "a **curadoria dos dados** usados no desenvolvimento e no aprimoramento de
inteligência artificial, adotando fontes de dados **seguras, rastreáveis e auditáveis**,
preferencialmente governamentais, permitida a contratação de fontes privadas, desde que
atendam aos requisitos de segurança e auditabilidade estabelecidos nesta Resolução…"

**Art. 2º, II** — "a transparência, a eficiência, a **explicabilidade**, a **contestabilidade**,
a **auditabilidade** e a confiabilidade das soluções…"

**Art. 7º** — "Os dados utilizados no desenvolvimento ou treinamento de modelos de inteligência
artificial devem ser representativos de casos judiciais e observar as cautelas necessárias
quanto ao **segredo de justiça** e à **proteção de dados pessoais**, nos termos da Lei nº
13.709/2018 (LGPD)."

## Uso de LLM comercial — as quatro travas do art. 19, §3º

**I** — "os usuários deverão realizar **capacitação e treinamentos específicos** sobre melhores
práticas, limitações, riscos, e uso ético, responsável e eficiente de LLMs…"

**III** ⭐ — "as **empresas fornecedoras** dos serviços de LLMs e IA generativa devem observar
padrões de política de proteção de dados e de propriedade intelectual… sendo **vedado o
tratamento, uso ou compartilhamento dos dados fornecidos pelos usuários do Poder Judiciário,
bem como dos DADOS INFERIDOS a partir desses, para treinamento, aperfeiçoamento ou quaisquer
outros fins não expressamente autorizados**."

**IV** ⭐ — "é **vedado o uso de LLMs e sistemas de IA generativa de natureza privada ou
externos ao Judiciário para processar, analisar, gerar conteúdo ou servir de suporte a decisões
a partir de documentos ou dados sigilosos ou protegidos por segredo de justiça**… **salvo
quando devidamente anonimizados NA ORIGEM** ou quando forem adotados mecanismos técnicos e
procedimentais que garantam a efetiva proteção e segurança desses dados e de seus titulares."

**V** — vedado o uso para as finalidades de **risco excessivo ou alto risco** (arts. 10 e 11).

**Art. 19, §2º** — quando o tribunal não oferece solução corporativa, é **facultada a contratação
direta** de solução por assinatura ou cadastro de natureza privada, observado o §3º.

**Art. 19, §§7º e 8º** — quem contratar solução de mercado **deverá prestar informações ao
respectivo tribunal**, que consolida e envia ao Comitê Nacional de IA do Judiciário.

## Treinamento com dado sigiloso — vedação expressa

**Art. 20** (trecho) — "É **vedada a utilização de dados sigilosos ou protegidos por segredo de
justiça para treinamento de modelos de inteligência artificial**, salvo prévia **anonimização
dos dados na origem**."

**Art. 20, II** — "o uso dos dados fornecidos pelos usuários… para treinamento fica condicionado
às bases legais da LGPD e não poderá ser utilizado para quaisquer outros fins não expressamente
autorizados, com realização de **monitoramento contínuo**…"

## Qualidade, segurança e ciclo de vida do dado (Capítulo VIII)

**Art. 26** — dados **preferencialmente de fontes públicas ou governamentais**, objeto de
**curadoria de qualidade**; usados dados de fonte não governamental, "deverá ser realizada uma
**verificação rigorosa da qualidade e segurança dos dados**". **§2º** — fonte não governamental
só quando a governamental for insuficiente ou inadequada. **§4º** ⭐ — "deverão ser coletados
apenas os dados **estritamente necessários** ao treinamento, **não devendo ser mantidos
conjuntos de dados sem uso ou controle quanto ao armazenamento**."

**Art. 27** ⭐ — "O sistema deverá **impedir que os dados recebidos sejam alterados** antes de
sua utilização no fluxo de desenvolvimento… por meio de mecanismos de **controle de versões,
tokens e registros para auditoria e monitoramento** que garantam a **integridade e
rastreabilidade dos dados**."

**Art. 28, §1º** — "O **isolamento** deverá assegurar que os dados do tribunal **não sejam
acessados, manipulados ou utilizados por terceiros sem autorização**…" · **III** — "adoção de
**criptografia robusta** para dados **em trânsito e armazenados**".

**Art. 29** — dados protegidos "contra os riscos de **destruição, modificação, extravio ou
acessos e transmissões não autorizados**, por meio de medidas técnicas e administrativas
adequadas."

**Art. 30** ⭐⭐ — "Nos casos em que o uso de soluções de inteligência artificial se dê
diretamente por meio de sítios eletrônicos, aplicativos ou **interfaces de programação de
aplicações (APIs)** que utilizem os dados compartilhados para **alimentar o repositório central
ou para fins de treinamento ou (re)adequação do modelo**, é **vedado o compartilhamento de dados
custodiados** pelo Judiciário, exceto quando esses dados forem **anonimizados ou
pseudoanonimizados na origem**…" **§2º** — mecanismos de auditoria e controle para verificar a
conformidade, "especialmente no uso de dados para fins de treinamento ou readequação".

**Art. 31, b)** ⭐ — "ao final do treinamento dos modelos, **eliminar os dados pessoais
não-anonimizados dos repositórios de dados (data lake, data warehouse ou data lakehouse)**…"
**d)** — "implementar a **governança e curadoria dos dados** utilizados, para garantir sua
qualidade e segurança".

## Supervisão humana e explicabilidade (Capítulo IX)

**Art. 32, II** — as soluções devem "possibilitar a **revisão detalhada do conteúdo gerado e dos
dados utilizados** para sua elaboração, assegurando que os usuários tenham **acesso às premissas
e ao método** empregado pela inteligência artificial na sua formulação, **sem que haja qualquer
espécie de vinculação à solução apresentada pela inteligência artificial** e garantindo-se a
possibilidade de correções ou ajustes."

**Art. 34** — "Os sistemas computacionais… deverão **exigir a supervisão humana** e permitir a
**modificação pelo magistrado competente de qualquer produto gerado pela inteligência
artificial**…"

## Governança, risco e prestação de contas

**Art. 9º** — avaliação de **grau de risco** por solução, conforme o **Anexo de Classificação de
Riscos**. **Art. 10** — vedações por **risco excessivo**; §2º — solução que passe a se enquadrar
nas vedações **deverá ser descontinuada**, com registro das razões. **Art. 14, §1º** —
**avaliação de impacto algorítmico** como processo **contínuo**, com auditorias regulares,
monitoramento contínuo, revisões periódicas e ações corretivas. **Art. 22** — governança de
dados + LGPD + LAI + propriedade intelectual + segredo de justiça; §2º — **relatórios
periódicos**. **Art. 24** — cadastro obrigatório no **Sinapses**. **Art. 42** — informar ao
Comitê Nacional **todos os eventos adversos**.
