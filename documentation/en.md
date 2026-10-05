<!-- ELUCENIA technical documentation · spesi · en · no clinical/professional/rights approval -->

# sPESI (simplified PESI)

[conditions, sources and permissions](https://elucenia.org/en/tools/spesi)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Age \> 80 years

`idade`

### Cancer (active or treated in the last year)

`cancer`

### Chronic cardiopulmonary disease (heart failure or chronic lung disease)

`cardiopulm`

### Heart rate ≥ 110 bpm

`fc`

### Systolic blood pressure \< 100 mmHg

`pas`

### O₂ saturation \< 90%

`sat`

## Method edition

sPESI/Jiménez 2010: 6 binary variables, 0 low risk, others high; not original 11-variable PESI

## Documented formula

One point each: age \> 80, cancer, chronic cardiopulmonary disease, HR ≥ 110, SBP \< 100, O₂ saturation \< 90%. 0 = low risk; ≥ 1 = high risk (sPESI).

## Limits and population

sPESI estimates prognosis in acute pulmonary embolism; it neither confirms nor excludes it. The study’s low-risk group still had deaths and does not independently authorize outpatient treatment. Instability, comorbidities, clinical factors and logistical conditions must be assessed within the corresponding protocol.

## References

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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
