# Exoplanet Exploration

![exoplanets.jpg](Images/exoplanets.jpg)

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system. The goal of this project is to create machine learning models capable of classifying candidate expoplanets from the raw dataset - [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

Steps taken:
1. Preprocess the raw data 
2. Tune the models
3. Compare two or more models

- - -

### Evaluation of Model Performance

Support Vector Machine:
* Testing score with default parameters: 0.852
* Testing score after hyperparameter tuning with GridSearchCV: 0.889

Random Forest Classifier:
* Testing score with default parameters: 0.852
* Testing score after hyperparameter tuning with GridSearchCV: **0.896

K Nearest Neighbors:
* Testing score with optimized k: 0.823

### Conclusion & Assumptions
The random forest classifier is the best model for this dataset. Generally, random forest classifiers should not be used to handle time-series data, because it doesn't fit well for increasing or decreasing trends. There is no formal distributional assumptions for random forests, they are non-parametric and can thus handle skewed and multi-model data as well as categorical data that are either ordinal or non-ordinal.
