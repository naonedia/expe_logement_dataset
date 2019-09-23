# expe_logement_dataset

## Datasets origins

* [DVF geolocated](https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres-geolocalisees/)
* [Evolution of gross disposable income and purchasing power](https://www.insee.fr/fr/statistiques/2830166#graphique-figure1)
* [OpenStreetMap Data](https://download.geofabrik.de/europe/france/pays-de-la-loire.html)

## Datasets available

### Neural networks

* `current_model`: contains current model used in production.

*N.B* the two data contained in COLUMNS_ORDER.csv are `mu` and `std` which are used to normalize data.

### Datasets

* `dvf_nantes_cleaned.csv`: Original DVF
* `origin_enriched_v2.csv`: DVF + POI
* `origin_enriched_v3.csv`: DVF + POI + Economy

#### origin_enriched_v4

DVF + POI + Economy. Postal code are fixe, we added Nantes district to get more details.
Contains longitude and latitude
* `origin_enriched_v4_lonlat.csv`

#### dataset_ready_v1

DVF + POI + Economy, data one-hot encoded, ready to use.
The second datasets has longitude and latitude for debugging purposes
* `dataset_ready_v1.csv`
* `dataset_ready_v1_lonlat.csv` 

#### dataset_ready_v2

DVF + POI + Economy, data one-hot encoded, ready to use.
Postal code are fixe, we added Nantes district to get more details.
Removed surface area < 25 m²
Removed housing outside of this range: in 50k€ < price < 1M€
Removed housing where price are less than 1600€/m²
Removed housing where they had same size, sold date, longitude and latitude.
The second datasets has longitude and latitude for debugging purposes
* `dataset_ready_v2.csv`
* `dataset_ready_v2_lonlat.csv`

### Finance

* `finance.csv`: Original data
* `finance_modified.csv`: Evolution of economy starting from 1st quarter of 2000. All other quarters are based on it.

### Others

* `code_postaux.csv`: Postal code associated to town (yes we have same postal code for differents town ¯\\\_(ツ)\_/¯ )
  

## Acknowledgement

“Ministry of Economy and Finance — Original data downloaded from https://www.data.gouv.fr/fr/datasets/demandes-de-valeurs-foncieres-geolocalisees/ updated on 25w April 2019”