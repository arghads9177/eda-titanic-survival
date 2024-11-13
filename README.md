# Titanic Passenger Survival Prediction

## Project Overview

This project focuses on predicting whether a passenger survived the sinking of the Titanic based on various features like ticket class, age, gender, and family relations aboard the ship. The dataset provides detailed information about each passenger, enabling the use of classification models to predict survival outcomes. This project demonstrates the use of machine learning classification techniques on one of the most famous datasets in the field of data science.

## Dataset Description

The dataset contains the following columns:

- **passengerid**: A unique identification number for each passenger.
- **survived**: Survival (0 = No, 1 = Yes)
- **Nmae**: Name of each passenger.
- **pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **sex**: Gender of the passenger
- **age**: Age of the passenger in years
- **sibsp**: Number of siblings/spouses aboard the Titanic
- **parch**: Number of parents/children aboard the Titanic
- **ticket**: Ticket number
- **fare**: Passenger fare
- **cabin**: Cabin number
- **embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

### Variable Notes

- **pclass**: A proxy for socio-economic status (SES)
  - 1st = Upper class
  - 2nd = Middle class
  - 3rd = Lower class

- **age**: Age is fractional if less than 1. If the age is estimated, it is in the form of `xx.5`.

- **sibsp**: Number of siblings/spouses aboard the Titanic.
  - Sibling = brother, sister, stepbrother, stepsister
  - Spouse = husband, wife (mistresses and fiancés were ignored)

- **parch**: Number of parents/children aboard the Titanic.
  - Parent = mother, father
  - Child = daughter, son, stepdaughter, stepson
  - Some children traveled only with a nanny, therefore `parch=0` for them.

## Objective

The goal of this project is to build a classification model that predicts the survival of passengers aboard the Titanic based on the provided features. The project includes data exploration, feature engineering, model building, and evaluation of classification models.

## Steps Involved:

1. **Data Exploration**: Explore the dataset to understand the distribution of variables and relationships between features and survival.
2. **Data Cleaning**: Handle missing data, especially in columns like `age`, `fare`, and `cabin`.
3. **Feature Engineering**: Create new features like family size, title from the passenger name, or binning of ages.

## Possible Model Choices

- **Logistic Regression**: A simple yet effective model for binary classification tasks.
- **Random Forest**: A powerful ensemble learning method that builds multiple decision trees and aggregates the results.
- **Support Vector Machines (SVM)**: A robust classifier for binary tasks, especially when the data is not linearly separable.
- **K-Nearest Neighbors (KNN)**: A non-parametric method that predicts the survival based on the closest neighbors in the feature space.

## Metrics for Evaluation

- **Accuracy**: Percentage of correctly predicted instances.
- **Precision**: Ratio of true positives to the total predicted positives.
- **Recall**: Ratio of true positives to the total actual positives.
- **F1-Score**: Harmonic mean of precision and recall.
- **ROC-AUC Score**: Area under the receiver operating characteristic curve, which measures the performance of the classification models across all threshold values.

## Conclusion

The **Titanic Passenger Survival Prediction** project aims to demonstrate how machine learning models can be applied to solve real-world classification problems. By analyzing and processing the Titanic dataset, we can build models that accurately predict which passengers were more likely to survive based on the available data.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/titanic-survival-prediction.git
