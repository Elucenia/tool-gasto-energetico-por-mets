<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · it · no clinical/professional/rights approval -->

# Dispendio energetico dai MET

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/gasto-energetico-por-mets)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Intensità dell’attività (valore del Compendium)

`met`

METs · intervallo: 1–25

### Peso

`peso`

kg · intervallo: 20–300

### Durata della sessione

`min`

min · intervallo: 1–600

### Sessioni alla settimana

`sessoes`

facoltativo · intervallo: 1–14

## Edizione del metodo

MET standard 3,5 mL O₂/kg/min; kcal/min=MET×3,5×kg/200; riferimento Compendium 2024

## Formula documentata

kcal/min = MET × 3,5 × peso (kg) ÷ 200 (1 MET = 3,5 mL O2/kg/min; circa 5 kcal per litro O2).

MET-min = MET × minuti. Approssimazione equivalente: kcal ≈ MET × peso (kg) × ore.

## Limiti e popolazione

I MET del Compendio per adulti 2024 corrispondono ad attività per adulti di 19–59 anni; i dati di persone di età ≥60 anni sono stati esclusi da tale edizione. I valori standardizzati, compresi quelli stimati, non misurano il dispendio individuale. Bambini, anziani e condizioni cliniche speciali richiedono fonti e metodi adeguati a tali popolazioni.

## Riferimenti

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
