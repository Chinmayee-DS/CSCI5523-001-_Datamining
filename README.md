
# Acute Liver Failure Prediction Model

## Project Overview
This repository houses the collaborative work on a data mining project aimed at developing a predictive model for Acute Liver Failure (ALF) among Indian adults. This model leverages a variety of machine learning techniques to analyze health-related data and predict ALF, contributing to better healthcare outcomes.

## Motivation
Our project seeks to advance the predictive capabilities for early diagnosis of Acute Liver Failure. By improving prediction accuracy, healthcare providers can offer timely and targeted treatments, potentially reducing the impact of ALF and enhancing patient care.

## Data Source
We utilized the "ALF Dataset" from Kaggle, which contains numerous health indicators such as cholesterol, blood pressure, BMI, and demographic data like age and gender. The initial dataset included 8750 entries, from which rows missing the target variable (ALF status) were removed, resulting in a final count of 6000 usable entries.

## Features
### Data Cleaning and Preprocessing
- **Handling Missing Values**: Employed techniques such as dropping missing data and imputing missing values using KNN for numerical and mode for categorical variables.
- **One-Hot Encoding**: Transformed categorical variables to a format suitable for modeling.

### Predictive Modeling Techniques
- **KNearestNeighbors and SMOTE**: Applied to selected features to balance the dataset and enhance the prediction model.
- **Random Forest and SMOTE**: Utilized for robust feature importance evaluation and predictive accuracy on balanced data.
- **Logistic Regression and SMOTE**: Used to predict the likelihood of ALF with selected features, providing insights into the impact of each feature.

### Feature Selection and Evaluation
- **ChiSq Selection**: Employed for categorical variables to determine the most significant predictors.
- **ANOVA Selection**: Used for continuous variables to assess the impact of each variable on the outcome.
- **Statistical Analysis**: Conducted to evaluate correlations and calculate odds ratios, especially for age as a predictor.

## Installation
To set up the project environment, follow these steps:

```bash
git clone https://github.com/anirxdh/CSCI5523-001-_Datamining.git
cd alf-prediction-project
pip install -r requirements.txt
```

## Usage
Execute the main analysis script or interact with the Jupyter notebook:

```bash
python main.py
```

or

```bash
jupyter notebook analysis.ipynb
```

## Contributing
Contributions are welcome. Please fork the repository and submit your pull requests for review.

