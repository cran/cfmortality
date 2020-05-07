[![Build Status](https://travis-ci.org/resplab/cfmortality.svg?branch=master)](https://travis-ci.org/resplab/cfmortality)
[![CRAN Status](https://www.r-pkg.org/badges/version/cfmortality)](https://CRAN.R-project.org/package=cfmortality)
[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)

## cfmortality
Allows clinicians to predict 1- and 2- year risk of death (with  a threshold risk of death of >= 20% for the 1-year model) in cyctic fibrosis patients based on patients' overal health status described in [https://erj.ersjournals.com/content/54/3/1900224](https://erj.ersjournals.com/content/54/3/1900224).


### Installation
You can install the latest development version from GitHub:

```
install.package("remotes")
remotes::install_github("resplab/cfmortality")
```

### Mortality Prediction

To get a prediction for mortality rate for first and second year , you will need to pass in patient's risk factors. For example: 

```
predictcfmortality (age = 16, male = 0, fvc = 66.7, fev1 = 47.4, fev1LastYear = 80.5, bcepacia = 0, underweight = 0, nHosp = 0, pancreaticInsufficient = 1, CFRelatedDiabetes = 0, ageAtDiagnosis = 0.9)

```

The **predictcfmortality()** function returns 1- year and 2-year mortality rate of patients with cystic fibrosis with 20% cut-off for risk of death of the 1-year model.

### Citation

Please cite: 

```
Stanojevic, Sanja, et al. "Development and external validation of 1-and 2-year mortality prediction models in cystic fibrosis." European Respiratory Journal 54.3 (2019): 1900224.
```
