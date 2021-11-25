# IMDB Rating Predictor ML Project

by Manasvi Singh, Pritish Wadhwa, Ananya Jain and Yash Bhargava, Machine Learning (CSE343, ECE343) from Indraprastha Institute of Information Technology, Delhi.

## Introduction

Is  it  possible  to  predict  the  rating  of  a  movie  prior  to  its release  or  production?   Every  year  countless  movies  are made and released worldwide.  All these movies are given ratings by viewers throughout the globe.These ratings are combined together to form the IMDb ratings.   IMDb rat-ing is the singlemost influential factor in deciding any con-sumer’s opinion and inherently the success of a movie.With the machine learning techniques at our disposal, we aim to predict the seemingly unpredictable IMDb rating ofany movie before its theatrical release. Successfully predicting IMDb rating is beneficial for both producers (from afinancial standpoint) and consumers (from an entertainment standpoint) alike.

## Description and Implementation Details
Steps performed:
-> Preprocessing : Removed skewed columns,Discarded NaN and null values, Discarded post release attributes and non informative attributes.

->Feature Selection: Using SkLearn K-Best Feature Selection, Correlation Matrix, Random Forest and Lasso Regression.

-> Hot Encoded Data and Normalized Data

## Models
Regression Models:
Linear Regression ,Lasso Regression, Ridge Regression ,Elastic Net and Support Vector Regression.

Classification Models:
Logistic Regression , Naive Bayes, Decision Trees, Random forest, K-nearest Neighbours,Support Vector Machines and Artificial Neural Network.

## Analysis
A number of models were trained for the task for both Re-gression  and  Classification.   For  regression  the  best  performing  model  was  Ridge.We  infer  that  most  of  thefeatures  selected  after  processing  data  are  important  asRidge outperforms other linear regressors.   For classification, SVM was the star performer.  Basic neural networkswere also tried but SVM outperformed them all. This mightbe because of SVM’s ability of extrapolating the featuresto  higher  dimensions  thus  making  the  classification  moreprominent.

## Conclusion
Our expectations from the project were to predict the IMDbrating of any movie using features that are available priorto its release and analyse the discriminatory power of fea-tures to analyse how different parameters impact the ratingfor any movie using various machine learning models.We  observed  that  features  like  length  of  a  movie,  the  di-rector, movie genres are amongst the most important onesto make any kind of prediction.  We also explored variousfeatures like the movie poster, the movie overview, the language of the movie and the country of production and foundout that even though they play an important part in the predictions, when taken individually they are not as strong asthe ones mentioned above.
