# OECD 2018 PISA Data

## Introduction

This folder contains data and analysis for the 2018 PISA scores and related country specific educational statistics taken from the OECD website, [data.oecd.org](https://data.oecd.org/).

## Contents

There are three notebooks and three datasets.

### Notebooks

* `international_edu_stats.ipynb` contains code for pulling raw data from data.oecd.org and building a comprehensive dataset, `full_educational_data.csv`.
* `international_ed_explore.ipynb` contains exploratory analysis of the `full_educational_data.csv` file. The notebook includes histograms, bar plots, a correlation heatmap, and feature importance scores calculated with the xgboost random forest algorithm.
* `international_ed_pca.ipynb` contains 2-factor and 3-fact primary component analysis (PCA) and visualizations for the educational data with PISA math scores as the dependent variable.

### Datasets

* `data_dictionary.csv` contains names, definitions, attributes, and detailed notes pertaining to the `full_educational_data.csv` file. It is best viewed in Excel or Google Sheets.
* `full_educational_data.csv` is the full dataset compiled from the raw OECD data. It contains 41 observations and 11 features. `PISASCIENCE`,`PISAMATH`, and `PISAREADING` are dependent variables.
* `country_codes.csv` contains the country ISO codes as described in the ISO 3166 international standard and full country names for easy identification of the observations in the full educational dataset. See [IBAN's country code page](https://www.iban.com/country-codes) for more information. 