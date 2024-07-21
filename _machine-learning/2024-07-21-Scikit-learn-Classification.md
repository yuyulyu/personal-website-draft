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

1. Import scikit-learn**
2. Build a model
3. Model learns from the labeled data (training data) passed to it
4. Pass unlabeled data to the model as input
5. Model predicts the labels of the unseen data

```python
from sklearn.module import Model
model = Model()
model.fit(X,y)
prediction = model.predict(X_new)
```

## K-Nearest-Neighbors
1. Initialisation
```python
from sklearn.neighbors import KNeighborsClassifier
X = training_data[["variable1","variable2"]].values
y = training_data[["output"]].values
```
2. Train model
```python
knn = KneighborsClassifier(n_neighbors=15)
knn.fit(X,y)
```
## Measuring model performance
$ accuracy = \frac{correct predictions}{total observations}$

