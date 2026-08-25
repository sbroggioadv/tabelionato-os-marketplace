---
name: emolumentos-norma-da-uf
description: "Roteia emolumentos para a lei, o índice, o ato temporal e as parcelas externas da UF, com atenção às arquiteturas anômalas do DF, RR, PB e GO e sem informar quantia em reais. Esta skill deve ser usada quando o pedido mencionar norma de emolumentos, tabela estadual, índice, atualização anual, TFJ, fundos, selo, ISS, ato vigente, lei-base, quanto custa ou qual tabela vale em determinada data e UF."
---

# Emolumentos — norma da UF

> Camada C2. Resolver a arquitetura estadual; delegar base e faixa à fundação C1. Zero valores em reais.

## Anexos e skill obrigatórios

- `context/emolumentos-norma-por-uf.md` — matriz das 27 arquiteturas;
- `context/uf-matriz-27.md` — documento-mãe, autoridade e anomalia resumida;
- `context/estado-da-norma.md` — corte temporal e alteradores;
- `context/travas-defasagem.md` — páginas antigas, leis suspensas e mudanças de regime;
- `emolumentos-a-base-nunca-o-valor` — piso federal, espécie, base e faixa.

Manter as 27 arquiteturas no anexo. Não reproduzir a matriz completa nesta skill nem na resposta.

## Entradas bloqueantes

Fixar UF, espécie do ato e data juridicamente relevante. Para análise de base, exigir ainda os documentos que provem conteúdo financeiro, valor declarado, avaliação fiscal/venal ou outra base prevista na lei local.

Sem UF, explicar somente a Lei 10.169/2000 e declarar que ela não escolhe a tabela estadual. Sem data, não escolher ato de atualização. Sem documento, não estimar base.

## Algoritmo

### 1. Localizar a arquitetura

Ler apenas a linha da UF em `emolumentos-norma-por-uf.md` e extrair:

- lei-base e alterações;
- índice ou mecanismo de atualização;
- ato vigente para o período;
- tabela ou item de Notas;
- notas explicativas;
- fundos, taxas, selo, ISS e parcelas externas;
- lacuna, suspensão ou transição.

Não usar lei de custas judiciais como lei extrajudicial. Não substituir ato vigente por notícia, página de listagem ou PDF desatualizado.

### 2. Aplicar o piso federal

Usar `emolumentos-a-base-nunca-o-valor` para:

- distinguir ato com e sem conteúdo financeiro;
- vedar percentual sobre o valor do negócio;
- vedar quantia fora da tabela;
- vedar cobrança por correção de erro do próprio serviço;
- escolher base/faixa somente quando a lei local autorizar;
- exigir recibo e identificação das parcelas.

Não informar preço, alíquota, orçamento ou total.

### 3. Resolver as quatro arquiteturas anômalas

- **DF:** aplicar a Lei federal 14.756/2023; ato fora da tabela é gratuito, inclusive sem analogia criativa.
- **RR:** usar a lei aplicável indicada no anexo e declarar que a Lei 1.157/2016 está suspensa, não revogada.
- **PB:** separar atos de 2026, sob a Lei 5.672/1992, do regime da Lei 14.343/2026, exigível somente em 2027.
- **GO:** identificar a versão da tabela válida na data, pois pode haver mais de uma mudança no mesmo ano; citar número com ano.

### 4. Separar parcelas externas

Não dizer que emolumento equivale ao total pago. Destacar, conforme a UF:

- RR: cinco colunas da arquitetura local;
- RN: cinco rubricas;
- SE: Taxa de Fiscalização e FERD;
- MG: emolumentos e TFJ como cobranças distintas;
- SC: FRJ em coluna separada;
- ES: FARPEN e FUNEPJ.

Aplicar a mesma separação a outros fundos, selo e ISS que a linha estadual indicar.

### 5. Fixar a temporalidade

Determinar o evento que escolhe a tabela: protocolo, apresentação, lavratura ou outro marco local. Conferir transição, início de vigência e alteração superveniente. Em SC, distinguir lavratura notarial de apresentação registral; em MT, preservar a regra para atos protocolizados antes da tabela nova; em SP, observar a vigência legal ligada à UFESP.

### 6. Declarar lacunas

Em ato ou índice não localizado, fornecer lei-base e caminho oficial sem completar o campo. Em RO, declarar a norma-mãe não localizada e a cobertura parcial. Não congelar valor, índice ou tabela em memória.

## Cartão de saída

| Campo | Resultado |
|---|---|
| UF, ato e data relevante | |
| lei-base | |
| índice/mecanismo | |
| ato de atualização | |
| tabela/item de Notas | |
| evento temporal | |
| espécie e base normativa | |
| fundos, taxas, selo e ISS | |
| anomalia ou transição | |
| lacuna/consulta necessária | |

Encerrar com: **“Este resultado identifica a norma e a arquitetura; consultar a tabela oficial vigente para obter a quantia.”**

## Reprovação automática

- informar valor em reais, percentual ou alíquota;
- escolher tabela sem UF e data;
- tratar emolumento como total pago;
- ocultar fundo, taxa, selo ou ISS;
- chamar a lei do DF de estadual;
- chamar lei suspensa de revogada em RR;
- aplicar a lei de 2027 a ato de 2026 na PB;
- presumir uma única tabela anual em GO;
- usar notícia ou página antiga como ato vigente;
- preencher a lacuna de RO por analogia.
