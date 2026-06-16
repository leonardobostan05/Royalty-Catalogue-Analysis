# Royalty Catalogue Analysis

> Welcher Produktionstyp ist für einen Musikproduzenten finanziell wertvoller:
> **kleine Anteile an großen Songs** oder **große Anteile an kleinen Songs**?
> Eine Analyse meines eigenen Tantiemen-Katalogs mit insgesamt 114 Songs.

<!-- HINWEIS AN DICH (vor dem Push löschen): Jeder Abschnitt unten mit [...] ist ein
Platzhalter, den du am Ende mit echten Ergebnissen füllst. Schreib das README ZULETZT,
wenn die Analyse steht — dann fällt es leicht, weil du die Antworten schon hast. -->

## Fragestellung

Als Produzent arbeite ich sowohl an größeren Projekten wie z.B. Netflix Shows mit vielen Beteiligten, wodurch meine Anteile an der Komposition kleiner werden, als auch an kleineren Projekten mit einem einzigen Künstler, wodurch mein Eigenanteil größer wird. Diese Analyse untersucht anhand realer, von mir über die Jahre angesammelter Daten:

1. Welcher Projekttyp hat mir historisch **mehr Einnahmen** gebracht?
2. Wie **konzentriert** ist mein Einkommen?
3. Was **charakterisiert** meine Top-Songs?

## Daten

- Quelle: Publishing Abrechnungen (Score & Beatstars) im Zeitraum Juni 2022 - Juni 2026
- Einheit der Analyse: ein Song (Werk).
- Zielgröße: mir zustehende Einnahmen in USD.
- Abgeleitete Kennzahl: **„wahre Songgröße" ≈ Einnahme ÷ Eigenanteil %**
  (Näherung der gesamten Tantiemen Masse eines Songs, unabhängig von meiner Scheibe).

> **Anmerkung zum Datenschutz:** Die echten Abrechnungsdaten sind nicht Teil dieses Repository
> (siehe `.gitignore`). Zum Nachvollziehen liegt ein anonymisierter Beispieldatensatz
> in `data/raw/sample/`.

## Methodik

[... kurz: Einlesen → Bereinigen → Anteile zusammenführen → „wahre Größe" berechnen
→ Pareto- und Gruppenvergleich → Visualisierung ...]

## Ergebnisse

[... 2–4 Kernbefunde mit Zahlen, z. B. „Top 10 % der Songs = XX % des Einkommens".
Die wichtigsten 2–3 Diagramme aus `figures/` hier einbetten. ...]

## Wichtigste Einschränkungen

- Die Daten messen **Einnahmen**, nicht Streams oder Hörverhalten.
- „Wahre Größe" ist eine **Näherung**, denn Teilen durch kleine Anteile verstärkt Fehler.
- Die Analyse ist **rückblickend beschreibend**, nicht kausal. Diese zeigt, was sich
  bisher gelohnt hat, nicht zwingend, welche Strategie künftig optimal ist.

## Reproduzieren

```bash
pip install -r requirements.txt
jupyter notebook notebooks/01_analysis.ipynb
```

## Tech-Stack

Python · pandas · matplotlib · Jupyter
