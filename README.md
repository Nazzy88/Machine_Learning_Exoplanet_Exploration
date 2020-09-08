# Machine_Learning_Exoplanet_Exploration
Processing NASA Kepler space telescope data through machine learning models capable of classifying candidate exoplanets from the raw dataset.

![exoplanets.jpg](Images/exoplanets.jpg)

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

In this project, you will need to:

1. [Preprocess the raw data](#Preprocessing)
2. [Tune the models](#Tune-Model-Parameters)
3. [Compare two or more models](#Evaluate-Model-Performance)

- - -

## Instructions

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

### Reporting

* Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).

## SVC
```
                precision    recall  f1-score   support

     CANDIDATE       0.76      0.61      0.68       422
     CONFIRMED       0.69      0.79      0.74       450
FALSE POSITIVE       0.99      1.00      0.99       876

      accuracy                           0.85      1748
     macro avg       0.81      0.80      0.80      1748
  weighted avg       0.85      0.85      0.85      1748

```
## SVC with Hyperparameter Tuning

```
                precision    recall  f1-score   support

     CANDIDATE       0.84      0.71      0.77       422
     CONFIRMED       0.76      0.86      0.80       450
FALSE POSITIVE       0.99      1.00      0.99       876

      accuracy                           0.89      1748
     macro avg       0.86      0.85      0.86      1748
  weighted avg       0.89      0.89      0.89      1748
  
  ```
  
  ## Random Forest
  
  ```
                precision    recall  f1-score   support

     CANDIDATE       0.76      0.84      0.80       378
     CONFIRMED       0.85      0.82      0.84       469
FALSE POSITIVE     1.00      0.97      0.98       901

      accuracy                           0.90      1748
     macro avg       0.87      0.88      0.87      1748
  weighted avg       0.91      0.90      0.90      1748
  
  ```
 ## Random Forest with Hyperparameter Tuning
  
  ```
                precision    recall  f1-score   support

     CANDIDATE       0.84      0.75      0.79       422
     CONFIRMED       0.81      0.86      0.83       450
FALSE POSITIVE     0.97      1.00      0.99       876

      accuracy                           0.90      1748
     macro avg       0.88      0.87      0.87      1748
  weighted avg       0.90      0.90      0.90      1748
  
  ```
  ## Gradient Boosting
  ```
                  precision    recall  f1-score   support

     CANDIDATE       0.85      0.79      0.82       422
     CONFIRMED       0.82      0.85      0.83       450
FALSE POSITIVE     0.99      1.00      0.99       876

      accuracy                           0.91      1748
     macro avg       0.88      0.88      0.88      1748
  weighted avg       0.91      0.91      0.91      1748
  ```
  ## Gradient Boosting with Hyperparameter Tuning
  
  ```
                precision    recall  f1-score   support

     CANDIDATE       0.84      0.80      0.82       422
     CONFIRMED       0.82      0.85      0.83       450
FALSE POSITIVE     0.99      1.00      1.00       876

      accuracy                           0.91      1748
     macro avg       0.88      0.88      0.88      1748
  weighted avg       0.91      0.91      0.91      1748
  ```
 
- - -

## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)

- - -
