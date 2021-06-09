# Covid-19-Rise-in-infection-regression-model

## Data Processing And Filtration

The dataset for this project originates from the [Our World In Data (Cases)](https://ourworldindata.org/covid-cases). The dataset has almost 26k entries and each of the 26k entries represent data about 33 features for Covid-19 cases for all countries uptill `'25-June-2020'`. For the purposes of this project, the following preprocessing steps have been made to the dataset:
- Out of 33 features 4 important features `'new_tests'`, `'population'`, `'population_density'` and   `'median_age'` have been selected for this project.
- All those selected data points which contain **missing or censored values** have been removed.
- Some data points in `'new_cases'` label have been considered as **outliers** and have been removed.
- After the removal of all the missing entries, 6.4k entries left in the dataset which have been used in the training and testing of the model.


### Data Processing and Feature Analysis
Data preprocessing and feature analysis notebooks can be found inside ```feature analysis``` folder. In that folder there are 2 files. In ```Feature distribution and plotting.ipynb ``` notebook you can find the ```univariate and bivariate``` analysis of features. The other file ```Missing values and imputations.ipynb``` is used for finding missing values and testing different technqiues of imputation. 


## Regression Model
Regression model for this project can be found inside ```model_documentation``` folder. I have used ```Decision Tree``` model and got 85.9% accuracy on testing data.

![Model Result](https://github.com/abdul789150/Covid-19-Rise-in-infection-regression-model-/blob/master/model_documentation/model-output.png)


### Libraries Required to run this project
For running this project following libraries are required:
* numpy
* pandas
* sklearn (sickit-learn)
* matplotlib
* IPython
* graphviz
