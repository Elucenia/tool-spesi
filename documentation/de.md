<!-- ELUCENIA technical documentation · spesi · de · no clinical/professional/rights approval -->

# sPESI (vereinfachter PESI)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/spesi)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Alter \> 80 Jahre

`idade`

### Krebs (aktiv oder im letzten Jahr behandelt)

`cancer`

### Chronische Herz-Lungen-Erkrankung (Herzinsuffizienz oder chronische Lungenerkrankung)

`cardiopulm`

### Herzfrequenz ≥ 110 bpm

`fc`

### Systolischer Blutdruck \< 100 mmHg

`pas`

### O₂-Sättigung \< 90%

`sat`

## Fassung der Methode

sPESI/Jiménez 2010:6 binäre Variablen,0 niedrig sonst hoch; kein Original-PESI mit 11 Variablen

## Dokumentierte Formel

Je ein Punkt: Alter \>80, Krebs, chronische Herz-Lungen-Krankheit, HF≥110, systolisch\<100, O₂-Sättigung\<90%. 0 = niedriges Risiko; ≥ 1 = hohes Risiko (sPESI).

## Grenzen und Population

sPESI schätzt die Prognose bei akuter Lungenembolie, bestätigt oder verneint diese aber nicht. Auch die Niedrigrisikogruppe der Studie hatte Todesfälle und erlaubt allein keine ambulante Behandlung. Instabilität, Begleiterkrankungen, klinische Faktoren und logistische Bedingungen müssen im entsprechenden Protokoll bewertet werden.

## Referenzen

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Niedriges Risiko: 30-Tage-Mortalität von 1,0%

Kandidat für eine frühe Entlassung oder eine Behandlung zu Hause, sofern keine anderen Hindernisse bestehen (Hestia-Kriterien).


### 2

Kein niedriges Risiko: 30-Tage-Mortalität von 10,9%

Intermediäres Risiko nach ESC: rechten Ventrikel beurteilen (Echo oder CT-Angiographie) und Troponin.


### 3

Kein niedriges Risiko: 30-Tage-Mortalität von 10,9%

Intermediäres Risiko nach ESC: rechten Ventrikel beurteilen (Echo oder CT-Angiographie) und Troponin.

