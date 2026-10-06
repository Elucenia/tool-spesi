<!-- ELUCENIA technical documentation · spesi · it · no clinical/professional/rights approval -->

# sPESI (PESI semplificato)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/spesi)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Età \> 80 anni

`idade`

### Cancro (attivo o trattato nell’ultimo anno)

`cancer`

### Malattia cardiopolmonare cronica (insufficienza cardiaca o malattia polmonare cronica)

`cardiopulm`

### Frequenza cardiaca ≥ 110 bpm

`fc`

### Pressione arteriosa sistolica \< 100 mmHg

`pas`

### Saturazione di O₂ \< 90%

`sat`

## Edizione del metodo

sPESI/Jiménez 2010:6 binarie,0 basso altrimenti alto; non PESI originale 11 variabili

## Formula documentata

Un punto per: età \>80, cancro, malattia cardiopolmonare cronica, FC≥110, PAS\<100, saturazione O₂\<90%. 0 = basso rischio; ≥ 1 = alto rischio (sPESI).

## Limiti e popolazione

L’sPESI stima la prognosi nell’embolia polmonare acuta, non la conferma né la esclude. Il gruppo a basso rischio dello studio ha comunque presentato decessi e non rappresenta un’autorizzazione autonoma al trattamento ambulatoriale. Instabilità, comorbilità, fattori clinici e condizioni logistiche devono essere valutati nel protocollo corrispondente.

## Riferimenti

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Basso rischio: mortalità a 30 giorni dell'1,0%

Candidato per dimissione precoce o trattamento domiciliare, se non vi sono altri impedimenti (criteri di Hestia).


### 2

Non è a basso rischio: mortalità a 30 giorni del 10,9%

Rischio intermedio secondo ESC: valutare il ventricolo destro (ecocardiogramma o angio-TC) e la troponina.


### 3

Non è a basso rischio: mortalità a 30 giorni del 10,9%

Rischio intermedio secondo ESC: valutare il ventricolo destro (ecocardiogramma o angio-TC) e la troponina.

