# IMDb Movie Rating Predictor ML Project

by **Ananya Jain**, **Manasvi Singh**, **Pritish Wadhwa** and **Yash Bhargava**, Machine Learning (CSE343/ECE343) under the guidance of **Dr. Jainendra Shukla** from **Indraprastha Institute of Information Technology, Delhi**.

## Introduction
<p align="justify">Is it possible to predict the rating of a movie prior to its release or production? Every year countless movies are made and released worldwide. All these movies are given ratings by viewers throughout the globe.These ratings are combined together to form the IMDb ratings. IMDb rating is the singlemost influential factor in deciding any consumer’s opinion and inherently the success of a movie.  

With the machine learning techniques at our disposal, we aim to predict the seemingly unpredictable IMDb rating of any movie before its theatrical release. Successfully predicting IMDb rating is beneficial for both producers (from a financial standpoint) and consumers (from an entertainment standpoint) alike.</p>

## Dataset
Links to original dataset: [Movie Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset), [Poster Dataset](https://www.kaggle.com/neha1703/movie-genre-from-its-poster)  
Link to preprocessed, train, val and test dataset: [Complete Dataset](https://drive.google.com/drive/folders/1m_SktiYKrOgIWUBiEIDZXnwItp7SZPPF?usp=sharing)

## Models
- Regression Models:
  - Linear Regression
  - Lasso Regression
  - Ridge Regression
  - ElasticNet
  - Support Vector Regression

- Classification Models:
  - Logistic Regression
  - Naive Bayes
  - Decision Trees
  - Random forest
  - K-nearest Neighbours
  - Support Vector Machines
  - Artificial Neural Network

## Repository Description
- ### Preprocessing
  Code files for preprocessing data, EDA, feature selection, encoding, train-val-test split and feature scaling
- ### Regression
  Code files for training, validating, generating graphs and saving regression models
- ### Classification
  Code files for training, validating, generating graphs and saving classification models
- ### Reports
  Proposal, Interim Report and Final Report
- ### Images
  Images used in reports

## How to run model ?
Link to saved models: [Models](https://drive.google.com/drive/folders/1R6wdDw_7IYnxOpSKZIfgcL329PNPD5Tf?usp=sharing)

- To load a model
  - .sav model
    ```python
    filename = 'model_name.sav'
    loaded_model = pickle.load(open(filename, 'rb'))
    ```
  - .h5 model
    ```python
    # for example: Sequential() model
    
    from keras.models import Sequential
    from keras.layers import Dense, Dropout, Flatten, Input, Convolution2D, MaxPooling2D, Dropouts  
    
    filename = 'model_name.h5'
    loaded_model = Sequential()
    loaded_model.add(Dense(250, activation='relu', input_dim=3561))
    loaded_model.add(Dropout(0.4))
    loaded_model.add(Dense(500, activation='relu'))
    loaded_model.add(Dropout(0.8))
    loaded_model.add(Dense(500, activation='relu'))
    loaded_model.add(Dropout(0.4))
    loaded_model.add(Dense(200, activation='relu'))
    loaded_model.add(Dropout(0.4))
    loaded_model.add(Dense(80, activation='relu'))
    loaded_model.add(Dense(21, activation='softmax'))
    loaded_model.compile(loss='categorical_crossentropy', optimizer='adam', metrics=['accuracy'])
    loaded_model.load_weights(filename)
    ```
- To test a model
  - .sav model
    ```python
    loaded_model.predict(test_X)
    ```
  - .h5 model
    ```python
    loaded_model.predict(test_X)
    ```
- To generate graphs
  - Steps to plot graphs are documented in the .ipynb files for respective models

## Contact
For further queries feel free to reach out to following contributors.  
Ananya Jain (ananya19408@iiitd.ac.in)  
Manasvi Singh (manasvi19369@iiitd.ac.in)  
Pritish Wadhwa (pritish19440@iiitd.ac.in)  
Yash Bhargava (yash19289@iiitd.ac.in)

## Final Report
![Final Report](/Reports/Report_Group2.pdf)
