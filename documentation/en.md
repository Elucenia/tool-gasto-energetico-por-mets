<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · en · no clinical/professional/rights approval -->

# Energy expenditure from METs

[conditions, sources and permissions](https://elucenia.org/en/tools/gasto-energetico-por-mets)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Activity intensity (Compendium value)

`met`

METs · range: 1–25

### Weight

`peso`

kg · range: 20–300

### Session duration

`min`

min · range: 1–600

### Sessions per week

`sessoes`

optional · range: 1–14

## Method edition

Standard MET 3.5 mL O₂/kg/min; kcal/min=MET×3.5×kg/200; Compendium 2024 reference

## Documented formula

kcal/min = METs × 3.5 × weight (kg) ÷ 200 (1 MET = 3.5 mL O2/kg/min; about 5 kcal per litre of O2).

MET-min = METs × minutes. An equivalent approximation is kcal ≈ METs × weight (kg) × hours.

## Limits and population

METs in the 2024 Adult Compendium correspond to activities for adults aged 19–59 years; data from people aged ≥60 years were excluded from that edition. Standardized values, including estimated values, do not measure individual expenditure. Children, older adults and special clinical conditions require sources and methods suited to those populations.

## References

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Vigorous intensity (≥ 6 METs)

| Result details | |
| --- | --- |
| Energy expenditure per minute | 9.8 kcal/min |
| Session volume | 240 MET-min |


### 2

Moderate intensity (3 to 5,9 METs)

| Result details | |
| --- | --- |
| Energy expenditure per minute | 4.9 kcal/min |
| Session volume | 158 MET-min |
| Weekly volume | 630 MET-min/week (meets the goal of 500 to 1000) |


### 3

Light intensity (< 3 METs)

| Result details | |
| --- | --- |
| Energy expenditure per minute | 2.6 kcal/min |
| Session volume | 150 MET-min |

