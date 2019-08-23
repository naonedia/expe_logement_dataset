# expe_logement_dataset

## Datasets origins

* [DVF geolocated](https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres-geolocalisees/)
* [Evolution of gross disposable income and purchasing power](https://www.insee.fr/fr/statistiques/2830166#graphique-figure1)
* [OpenStreetMap Data](https://download.geofabrik.de/europe/france/pays-de-la-loire.html)

## Datasets available

### Datasets

* `dvf_nantes_cleaned.csv`: Original DVF
* `origin_enriched_v2.csv`: DVF + POI
* `origin_enriched_v3.csv`: DVF + POI + Economy
* `dataset_ready_v1.csv`: DVF + POI + Economy, data one-hot encoded, ready to use

### Finance

* `finance.csv`: Original data
* `finance_modified.csv`: Evolution of economy starting from 1st quarter of 2000. All other quarters are based on it.

### Others

* `code_postaux.csv`: Postal code associated to town (yes we have same postal code for differents town ¯\\\_(ツ)\_/¯ )
  

## Acknowledgement

“Ministry of Economy and Finance — Original data downloaded from https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres-geolocalisees/ updated on 25w April 2019”