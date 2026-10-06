<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · pt-BR · no clinical/professional/rights approval -->

# Gasto energético por METs

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/gasto-energetico-por-mets)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Intensidade da atividade (valor do Compendium)

`met`

METs · intervalo: 1–25

### Peso

`peso`

kg · intervalo: 20–300

### Duração da sessão

`min`

min · intervalo: 1–600

### Sessões por semana

`sessoes`

opcional · intervalo: 1–14

## Edição do método

METstandard 3,5 m LO 2/kg/min; kcal/min=MET×3,5×kg/200; referência Compendium 2024

## Fórmula documentada

kcal/min = METs × 3,5 × peso (kg) ÷ 200 (1 MET = 3,5 mL de O2/kg/min; cerca de 5 kcal por litro de O2).

MET-min = METs × minutos. Uma aproximação equivalente é kcal ≈ METs × peso (kg) × horas.

## Limites e população

Os METs do Compêndio Adulto 2024 correspondem a atividades para adultos de 19–59 anos; dados de pessoas ≥60 anos foram excluídos dessa edição. Valores padronizados, inclusive valores estimados, não medem gasto individual. Crianças, idosos e condições clínicas especiais exigem fontes e métodos adequados a essas populações.

## Referências

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Intensidade vigorosa (≥ 6 METs)

| Detalhes do resultado | |
| --- | --- |
| Gasto por minuto | 9,8 kcal/min |
| Volume da sessão | 240 MET-min |


### 2

Intensidade moderada (3 a 5,9 METs)

| Detalhes do resultado | |
| --- | --- |
| Gasto por minuto | 4,9 kcal/min |
| Volume da sessão | 158 MET-min |
| Volume semanal | 630 MET-min/semana (atinge a meta de 500 a 1.000) |


### 3

Intensidade leve (< 3 METs)

| Detalhes do resultado | |
| --- | --- |
| Gasto por minuto | 2,6 kcal/min |
| Volume da sessão | 150 MET-min |

