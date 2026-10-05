<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · de · no clinical/professional/rights approval -->

# Energieverbrauch nach MET

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/gasto-energetico-por-mets)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Aktivitätsintensität (Compendium-Wert)

`met`

METs · Bereich: 1–25

### Gewicht

`peso`

kg · Bereich: 20–300

### Dauer der Einheit

`min`

min · Bereich: 1–600

### Einheiten pro Woche

`sessoes`

optional · Bereich: 1–14

## Fassung der Methode

Standard-MET 3,5 mL O₂/kg/min; kcal/min=MET×3,5×kg/200; Compendium 2024

## Dokumentierte Formel

kcal/min = MET × 3,5 × Gewicht (kg) ÷ 200 (1 MET = 3,5 mL O2/kg/min; etwa 5 kcal pro Liter O2).

MET-min = MET × Minuten. Gleichwertige Näherung: kcal ≈ MET × Gewicht (kg) × Stunden.

## Grenzen und Population

Die MET-Werte des Erwachsenenkompendiums 2024 beziehen sich auf Aktivitäten von Erwachsenen von 19–59 Jahren; Daten von Personen ≥60 Jahre wurden aus dieser Ausgabe ausgeschlossen. Standardisierte Werte, einschließlich geschätzter Werte, messen keinen individuellen Verbrauch. Kinder, ältere Menschen und besondere klinische Situationen erfordern für diese Populationen geeignete Quellen und Methoden.

## Referenzen

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
