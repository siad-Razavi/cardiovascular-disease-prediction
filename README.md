# Cardiovascular Disease Prediction using Machine Learning

This project explores the use of supervised machine learning to predict the presence of cardiovascular disease from patient medical and lifestyle information. The goal is to identify whether a patient is likely to have cardiovascular disease based on non-invasive health indicators such as age, blood pressure, cholesterol, glucose level, and behavioral factors.

## Objective

The main objective of this project is to build and evaluate classification models that predict the target variable `cardio`, where:

- `0` = no cardiovascular disease
- `1` = cardiovascular disease

This project also focuses on understanding the impact of data cleaning, feature engineering, and model selection on predictive performance.

## Dataset

This project uses the **Cardiovascular Disease Dataset** available on Kaggle.

The dataset contains approximately **70,000 patient records** with medical and lifestyle-related features, including:

- age
- gender
- height
- weight
- systolic blood pressure
- diastolic blood pressure
- cholesterol
- glucose
- smoking
- alcohol intake
- physical activity

**Dataset source:**  
[Kaggle – Cardiovascular Disease Dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset/data)

## Project Workflow

The notebook includes the following main steps:

- data loading and inspection
- data cleaning
- removal of invalid and extreme blood pressure values
- exploratory data analysis (EDA)
- feature engineering
- correlation analysis
- train-test split
- feature scaling
- model training
- hyperparameter tuning
- model evaluation and comparison
- PCA-based additional analysis

## Feature Engineering

To improve the predictive power of the models, additional features were created, including:

- **BMI (Body Mass Index)** derived from height and weight
- **Pulse Pressure** derived from systolic and diastolic blood pressure
- **Age Groups** for analyzing cardiovascular risk across age ranges

## Models Used

The following machine learning models were trained and evaluated:

- Logistic Regression
- Random Forest
- K-Nearest Neighbors (KNN)
- Naive Bayes

Hyperparameter tuning was performed for the main models to improve performance.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Recall
- F1-score
- ROC-AUC

Additional visual analysis includes:

- confusion matrices
- ROC curves
- feature importance plots
- model performance comparison charts

## Results

The best-performing model in this project was the **tuned Random Forest**, which achieved approximately:

- **Accuracy:** 73.35%
- **Recall:** 67.96%
- **F1-score:** 71.58%
- **ROC-AUC:** 80.18%

The analysis also showed that blood pressure-related features such as `ap_hi`, `ap_lo`, and `pulse_pressure` were among the most important predictors.

## Key Insights

- Blood pressure features were the strongest predictors of cardiovascular disease.
- Feature engineering helped improve the representation of patient health information.
- Random Forest achieved the best overall performance among the tested models.
- PCA did not improve predictive performance in this case.

## Tools and Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Repository Contents

- `cardiovascular_disease_prediction.ipynb` — main notebook containing the full workflow
- `README.md` — project overview and summary

## How to Run

1. Download the dataset from Kaggle using the link above.
2. Place the dataset file in the appropriate project directory.
3. Open the notebook in Jupyter Notebook or VS Code.
4. Run the cells sequentially.

## Author

**Said Abolhassan Razavi**
