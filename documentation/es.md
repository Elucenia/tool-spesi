<!-- ELUCENIA technical documentation · spesi · es · no clinical/professional/rights approval -->

# sPESI (PESI simplificado)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/spesi)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Edad \> 80 años

`idade`

### Cáncer (activo o tratado en el último año)

`cancer`

### Enfermedad cardiopulmonar crónica (insuficiencia cardíaca o enfermedad pulmonar crónica)

`cardiopulm`

### Frecuencia cardíaca ≥ 110 bpm

`fc`

### Presión arterial sistólica \< 100 mmHg

`pas`

### Saturación de O₂ \< 90%

`sat`

## Edición del método

sPESI/Jiménez 2010:6 binarias,0 bajo riesgo, resto alto; no PESI original 11 variables

## Fórmula documentada

Un punto por: edad \>80, cáncer, enfermedad cardiopulmonar crónica, FC≥110, PAS\<100, saturación O₂\<90%. 0 = bajo riesgo; ≥ 1 = alto riesgo (sPESI).

## Límites y población

El sPESI estima el pronóstico en embolia pulmonar aguda, no la confirma ni la excluye. El grupo de bajo riesgo del estudio aún presentó muertes y no representa una autorización aislada de tratamiento ambulatorio. La inestabilidad, las comorbilidades, los factores clínicos y las condiciones logísticas deben evaluarse en el protocolo correspondiente.

## Referencias

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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
