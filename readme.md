# Kaggle Challenge - Titanic Survival Prediction

This project uses machine learning to predict passenger survival on the Titanic. It demonstrates data preprocessing, exploratory data analysis, and the application of a Random Forest Classifier to make predictions.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Making Predictions](#making-predictions)

## Prerequisites

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/titanic-survival-prediction.git
   ```
2. Navigate to the project directory:
   ```
   cd titanic-survival-prediction
   ```
3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Ensure you have the Titanic dataset files (`train.csv` and `test.csv`) in the project directory.
2. Run the main script:
   ```
   python titanic_prediction.py
   ```

## Features

- Data cleaning and preprocessing
- Exploratory data analysis with visualizations
- Feature engineering
- Model training using Random Forest Classifier
- Cross-validation for model evaluation
- Prediction on test data

## Data Preprocessing

- Handling missing values in 'Age' and 'Embarked' columns
- Creating new features: 'Sex_binary', 'AgeGroup', 'Fare_level', 'Title', 'Fam_size'
- Encoding categorical variables

## Exploratory Data Analysis

The script includes several visualization functions to explore the relationships between features and survival rates:

- `bar_chart_stacked()`: Creates stacked bar charts for categorical features
- `bar_chart_compare()`: Compares survival rates across different feature combinations
- `plot_distribution()`: Visualizes the distribution of numerical features

## Model Training and Evaluation

- Uses Random Forest Classifier with 500 estimators and max depth of 5
- Performs cross-validation using RepeatedKFold with 2 splits and 10 repeats
- Calculates and displays accuracy scores for each fold and the mean accuracy

## Making Predictions

The trained model is used to make predictions on the test dataset. The results are saved in a CSV file named 'Titanic_submission2.csv'.

---

Feel free to contribute to this project by opening issues or submitting pull requests!
