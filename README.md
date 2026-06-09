# Decision Tree Classification and Regression

## Overview

This repository contains two machine learning projects built using Scikit-Learn:

1. **Decision Tree Classification** using the Titanic dataset.
2. **Decision Tree Regression** using the Diabetes dataset.

The objective is to understand how Decision Trees work for both classification and regression problems, along with techniques for model tuning, pruning, evaluation, and visualization.

---

## Project 1: Decision Tree Classification (Titanic Dataset)

### Objective

Predict whether a passenger survived the Titanic disaster based on selected passenger features.

### Dataset

The Titanic dataset is loaded directly from the Seaborn library.

### Features Used

* Passenger Class (`pclass`)
* Gender (`sex`)
* Embarkation Port (`embarked`)
* Age (`age`)

### Target Variable

* Survival Status (`survived`)

### Steps Performed

#### 1. Data Exploration

* Loaded the Titanic dataset
* Checked dataset structure
* Identified missing values

#### 2. Data Preprocessing

* Filled missing age values using Median Imputation
* Filled missing embarkation values using Most Frequent Imputation
* Encoded categorical variables using Label Encoding

#### 3. Model Training

* Split dataset into training and testing sets
* Trained a Decision Tree Classifier

#### 4. Model Evaluation

* Calculated classification accuracy
* Compared performance for different tree depths

#### 5. Pre-Pruning Techniques

* Tuned:

  * `max_depth`
  * `min_samples_split`

#### 6. Post-Pruning Technique

* Applied Cost Complexity Pruning (`ccp_alpha`)
* Selected the best alpha value based on test accuracy

#### 7. Visualization

* Visualized the full decision tree
* Visualized the pruned decision tree

### Evaluation Metric

* Accuracy Score

---

## Project 2: Decision Tree Regression (Diabetes Dataset)

### Objective

Predict disease progression values using patient medical measurements.

### Dataset

The Diabetes dataset is loaded directly from Scikit-Learn.

### Features

The dataset contains 10 standardized medical predictor variables.

### Target Variable

* Disease Progression Score

### Steps Performed

#### 1. Data Preparation

* Loaded the Diabetes dataset
* Split data into training and testing sets

#### 2. Model Training

* Trained a Decision Tree Regressor
* Configured:

  * `max_depth = 7`
  * `min_samples_leaf = 20`

#### 3. Model Evaluation

* Predicted on training and testing datasets
* Calculated:

  * Mean Squared Error (MSE)
  * R² Score

#### 4. Visualization

* Visualized the regression tree structure

### Evaluation Metrics

* Mean Squared Error (MSE)
* R² Score

---

## Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn

---

## Key Concepts Covered

### Classification

* Decision Tree Classifier
* Missing Value Imputation
* Label Encoding
* Train-Test Split
* Hyperparameter Tuning
* Cost Complexity Pruning
* Tree Visualization

### Regression

* Decision Tree Regressor
* Mean Squared Error
* R² Score
* Tree Visualization

---

## Project Structure

```text
├── decision_tree_classifier.ipynb
├── decision_tree_regressor.ipynb
├── README.md
```

---

## Learning Outcomes

By completing this project, you will learn:

* How Decision Trees perform classification and regression tasks.
* How to preprocess real-world datasets.
* How to tune Decision Tree hyperparameters.
* How pruning helps reduce overfitting.
* How to evaluate models using appropriate metrics.
* How to visualize Decision Tree structures for better interpretability.

---

## Future Improvements

* Random Forest Classification
* Random Forest Regression
* Grid Search Hyperparameter Optimization
* Cross Validation
* Feature Importance Analysis
* Ensemble Learning Techniques

---

## Author

Created as part of a Machine Learning learning project using Python and Scikit-Learn.
