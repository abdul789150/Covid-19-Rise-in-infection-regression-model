# Covid-19-Rise-in-infection-regression-model

## Data Processing And Filtration

The dataset for this project originates from the [Our World In Data (Cases)](https://ourworldindata.org/covid-cases). The dataset has almost 26k entries and each of the 26k entries represent data about 33 features for Covid-19 cases for all countries uptill `'25-June-2020'`. For the purposes of this project, the following preprocessing steps have been made to the dataset:
- Out of 33 features 4 important features `'new_tests'`, `'population'`, `'population_density'` and   `'median_age'` have been selected for this project.
- All those selected data points which contain **missing or censored values** have been removed.
- Some data points in `'new_cases'` label have been considered as **outliers** and have been removed.
- After the removal of all the missing entries, 6.4k entries left in the dataset which have been used in the training and testing of the model.
