<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · es · no clinical/professional/rights approval -->

# Gasto energético por MET

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/gasto-energetico-por-mets)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Intensidad de la actividad (valor del Compendium)

`met`

METs · intervalo: 1–25

### Peso

`peso`

kg · intervalo: 20–300

### Duración de la sesión

`min`

min · intervalo: 1–600

### Sesiones por semana

`sessoes`

opcional · intervalo: 1–14

## Edición del método

MET estándar 3,5 mL O₂/kg/min; kcal/min=MET×3,5×kg/200; referencia Compendium 2024

## Fórmula documentada

kcal/min = METs × 3,5 × peso (kg) ÷ 200 (1 MET = 3,5 mL O2/kg/min; unos 5 kcal por litro de O2).

MET-min = METs × minutos. Aproximación equivalente: kcal ≈ METs × peso (kg) × horas.

## Límites y población

Los MET del Compendio Adulto 2024 corresponden a actividades para adultos de 19–59 años; los datos de personas de ≥60 años se excluyeron de esa edición. Los valores estandarizados, incluidos los estimados, no miden el gasto individual. Niños, personas mayores y condiciones clínicas especiales requieren fuentes y métodos adecuados para esas poblaciones.

## Referencias

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Intensidad vigorosa (≥ 6 METs)

| Detalles del resultado | |
| --- | --- |
| Gasto por minuto | 9,8 kcal/min |
| Volumen de la sesión | 240 MET-min |


### 2

Intensidad moderada (3 a 5,9 METs)

| Detalles del resultado | |
| --- | --- |
| Gasto por minuto | 4,9 kcal/min |
| Volumen de la sesión | 158 MET-min |
| Volumen semanal | 630 MET-min/semana (cumple el objetivo de 500 a 1000) |


### 3

Intensidad leve (< 3 METs)

| Detalles del resultado | |
| --- | --- |
| Gasto por minuto | 2,6 kcal/min |
| Volumen de la sesión | 150 MET-min |

