---
name: estado-e-tipo-do-provimento
description: "Classificador de atos do CNN em seis combinações: três estados normativos — absorvido/revogado, vivo por remissão e suspenso — cruzados com três tipos — alterador, autônomo e Resolução do Plenário. Esta skill deve ser usada antes de citar provimento ou resolução, ou quando o pedido mencionar norma revogada, suspensa, incorporada, ato autônomo, resolução fora do Código, Provimentos 172, 175, 247, 50, 56, 62, 103, 197, 213, estado da norma, vigência ou tipo do ato."
---

# Estado e tipo do provimento

> Camada C1. Resolver duas dimensões independentes antes de citar qualquer ato.

## Anexos obrigatórios

- `context/estado-da-norma.md`;
- `context/cnn-149-2023-compilado.md`;
- `context/travas-defasagem.md`.

## Dimensão 1 — estado

### Absorvido/revogado

O conteúdo foi incorporado/substituído no Código e o ato anterior não deve ser tratado como fonte operacional autônoma, salvo remissão viva ou necessidade histórica. Citar o artigo vigente do CNN e creditar a origem apenas quando útil.

### Vivo por remissão

O ato continua aplicável porque o próprio Código remete a ele. Na data de corte, exemplos confirmados:

- Provimento 56/2016 — RCTO;
- Provimento 103/2020 — AEV;
- Provimento 62/2017 — apostilamento/anexos;
- Provimento 50/2015 — temporalidade;
- Provimento 197/2025 — conta notarial;
- Provimento 213/2026 — TIC e acervo digital.

Citar o artigo do CNN que faz a ponte e o ato autônomo remetido.

### Suspenso

Tratar suspensão como terceiro estado, diferente de revogação. Na fotografia de 25/08/2026, constavam suspensos os Provimentos 172/2024, 175/2024 e 247/2026. O último exigia nova conferência por volta de 12/10/2026 🟡.

Aplicar a mesma lógica a norma estadual: a Lei RR 1.157/2016 sob ADI não vira “revogada”; a base aplicável continuava sendo a Lei 752/2009 na data de corte.

## Dimensão 2 — tipo

### Alterador

Modifica o texto do CNN. Citar o dispositivo consolidado e, quando necessário, indicar o provimento que deu a redação. Não construir corpus paralelo com todos os alteradores.

### Autônomo

Convive fora do CNN, com disciplina própria ou por remissão. Citar o ato e o artigo-ponte do Código quando houver. Vigiar atos autônomos separadamente; eles podem mudar sem aparecer na lista de alterações do Provimento 149.

### Resolução do Plenário

Permanece fora do CNN por competência do Plenário. Resoluções 35/2007 e 571/2024, por exemplo, não foram “absorvidas” pelo Código. Citar a Resolução como endereço próprio e o artigo do CNN que manda observá-la, quando houver.

## Classificação em seis valores

Registrar sempre:

```text
ato: espécie + número + ano
estado: absorvido_revogado | vivo_por_remissao | suspenso
tipo: alterador | autonomo | resolucao_plenario
ponte_cnn: artigo ou inexistente
redacao_aplicavel: dispositivo e origem
data_corte: DD/MM/AAAA
ressalva: nenhuma | checar_ao_vivo | conflito
```

Se o ato não couber honestamente em um dos três estados por falta de fonte, usar `estado_nao_confirmado`; não escolher por aparência.

## Método

1. Abrir a ficha/registro oficial do ato na base disponível.
2. Conferir situação declarada, revogador, suspensão e alterações.
3. Pesquisar o número no compilado e identificar remissão ou etiqueta de redação.
4. Identificar espécie e competência do órgão emissor.
5. Comparar data com `estado-da-norma.md`.
6. Emitir a ficha de classificação antes da citação substantiva.

## Travas duras

- Provimento 74/2018: revogado pelo 213/2026; remissão estadual morta não o ressuscita.
- Provimento 244/2026: não altera o CNN; o alterador de 21/07 é o 242.
- Provimentos 228 e 229: ambos existem; não tratar um como erro do outro.
- Texto empilhado: a última redação por data vence; ausência de tachado não mantém redações antigas.
- Exposição de Motivos: fotografia histórica, não gate atual.
- Suspensão: não converter em revogação nem eficácia plena.

## Entrega obrigatória

Entregar ficha dos seis valores, fundamento da classificação, artigo-ponte, data de corte e consequência de citação. Não interpretar o mérito do ato além do necessário para classificá-lo.
