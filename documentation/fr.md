<!-- ELUCENIA technical documentation · spesi · fr · no clinical/professional/rights approval -->

# sPESI (PESI simplifié)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/spesi)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Âge \> 80 ans

`idade`

### Cancer (actif ou traité dans la dernière année)

`cancer`

### Maladie cardiopulmonaire chronique (insuffisance cardiaque ou maladie pulmonaire chronique)

`cardiopulm`

### Fréquence cardiaque ≥ 110 bpm

`fc`

### Pression artérielle systolique \< 100 mmHg

`pas`

### Saturation en O₂ \< 90%

`sat`

## Édition de la méthode

sPESI/Jiménez 2010 :6 binaires,0 faible, reste haut ; pas PESI original 11 variables

## Formule documentée

Un point chacun: âge \>80, cancer, maladie cardiopulmonaire chronique, FC≥110, PAS\<100, saturation O₂\<90%. 0 = faible risque; ≥ 1 = haut risque (sPESI).

## Limites et population

Le sPESI estime le pronostic dans l’embolie pulmonaire aiguë, sans la confirmer ni l’exclure. Même le groupe à faible risque de l’étude comportait des décès et ne constitue pas une autorisation isolée de traitement ambulatoire. L’instabilité, les comorbidités, les facteurs cliniques et les conditions logistiques doivent être évalués dans le protocole correspondant.

## Références

- [Jiménez D et al. Simplification of the pulmonary embolism severity index for prognostication in patients with acute symptomatic pulmonary embolism. Arch Intern Med, 2010.](https://doi.org/10.1001/archinternmed.2010.199)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism developed in collaboration with the European Respiratory Society (ERS). Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Faible risque : mortalité à 30 jours de 1,0 %

Candidat à une sortie précoce ou à un traitement à domicile, s’il n’y a pas d’autres contre-indications (critères de Hestia).


### 2

Pas de faible risque : mortalité à 30 jours de 10,9 %

Risque intermédiaire selon l’ESC : évaluer le ventricule droit (échocardiographie ou angioscanner) et la troponine.


### 3

Pas de faible risque : mortalité à 30 jours de 10,9 %

Risque intermédiaire selon l’ESC : évaluer le ventricule droit (échocardiographie ou angioscanner) et la troponine.

