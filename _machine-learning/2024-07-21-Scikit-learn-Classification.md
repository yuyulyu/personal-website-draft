---
title: "Scikit-learn: Classification"
date: 2024-07-21
permalink: /machine-learning/DataCamp-Classification/
tags:
  - machine learning
  - scikit-learn
sidebar:
  - title: "Title"
    url: "#"
  - nav:
    - title: "Header two"
      url: “#header-two"
---

# Machine Learning with scikit-learn {#machine-learning-with-scikit-learn}

## Before using supervise learning
- **Requirements**
  - No missing values
  - Data in numeriv format
  - Data sorted in pandas DataFrame or NumPy array
- **Perform Exploratory Data Analysis (EDA) first**

## Scikit-learn Syntax

1. Import scikit-learn**.
   ```python
    from sklearn.module import Model
   ```
   K-Nearest-Neighbors:
   ```python
    from sklearn.neighbors import KNeighborsClassifier
   ```
2. Train/test split.
  ```python
  from sklearn.model_selection import train_test_split
  X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.3, random_state = 21 stratify = y)
  ``` 
4. Build a model.
  ```python
  model = Model()
  ```
   K-Nearest-Neighbors:
   ```python
    knn = KneighborsClassifier(n_neighbors=15)
   ```
6. Model learns from the labeled data (training data) passed to it.
  ```python
  model.fit(X,y)
  ```
   K-Nearest-Neighbors:
   ```python
    knn.fit(X,y)
   ```
8. Pass unlabeled data to the model as input, model predicts the labels of the unseen data.
  ```python
  prediction = model.predict(X_new)
  ```



