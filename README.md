## Table of Contents
1. [Project Motivation](#motivation)
2. [Summary of Results](#results)
3. [Libraries Used](#libraries)
4. [File Descriptions](#descriptions)
5. [Acknowledgements](#acknowledgements)

## Project Motivation <a name="motivation"></a>
### Customer Churn Prediction with Spark
Project Overview: Sparkify is a digital music service similar to Spotfiy and Pandora. In Sparkify, users can either listen to music for free or buy a subscription. Customer churn prevention is a hot and challenging problem in almost every product and service company. If companies were able to utilize customer-usage data to find unique trends and accurately map them to indicate which customers may churn, it would be possible to incentivize customers to remain using their services giving them a loyal customer base which is key for a company’s growth.
 
Project Purpose: In order to identify users who are likely to churn, it’s important to perform an exploratory analysis to glean insights from the data set and identify key variables of interest. The next process is to experiment different model algorithms and then select the best model based on key evaluation metric such as F1 Score and accuracy using Spark ML Library.

Data
The data we have from Sparkify is that of user events. Every interaction of every user with the application is given to us. This means every time a user goes to the Home page, listens to a song, thumbs up a song, etc. we have an event in the data corresponding to the same.


## Summary of Results <a name="results"></a>
We fitted logistic regression, Random Forest Gradient boosting and Decision Tree classifier with default parameter. We'll look for f1 score and accuracy, however f1 score is more reliable in this case due to imbalance in class from accuracy. The table summarised the scores for these classifiers and logistic regression tuned.

| Classifier      | f1-score | accuracy |
| -------------   | ------:| -------:|
| Logistic Regression|0.92740|0.92887|
| Random Forest      |0.92187|0.92993|
| Gradient Boosting |0.98821|0.98832|
| Decision Tree|0.94152|0.90552|
| Logistic Regression Tuned|0.89731|0.90552|

With the default parameter, Gradient Boosting has the highest score of all the metrics and Logistic Regression comes second.

## Libraries and Dependencies: <a name="libraries"></a>

Python 3.6.6+, Spark

1. pandas
2. numpy
3. matplotlib
4. time, datetime 
5. scikit-learn
6. pyspark.sql
7. pyspark.ml

## File Descriptions <a name="descriptions"></a>

1. Sparkify.ipynb - Jupyter notebook containing Spark implementation.
2. README.md (this file)

## Acknowledgements <a name="acknowledgements"></a>
1. https://www.udacity.com/
