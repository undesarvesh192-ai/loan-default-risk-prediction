# 🏦 Loan Default Risk Prediction

A Machine Learning project that predicts the risk of a borrower defaulting on a loan using financial and personal information.

## 📌 Project Overview

Loan default prediction helps financial institutions identify borrowers who may have difficulty repaying loans. This project uses machine learning algorithms to estimate the probability of loan default.

The project includes data analysis, preprocessing, model training, evaluation, and an interactive web interface built with Gradio.

## 🎯 Objectives

* Predict whether a borrower may default on a loan.
* Explore borrower data and identify useful patterns.
* Compare different machine learning algorithms.
* Evaluate models using classification metrics.
* Provide predictions through a simple web interface.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Gradio
* Google Colab
* Joblib

## 🤖 Machine Learning Models

Three algorithms were trained and evaluated:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

Random Forest was selected for the interactive prediction interface.

## 📊 Model Evaluation

The Random Forest model achieved the following results at the default classification threshold of 0.50:

| Metric              |  Score |
| ------------------- | -----: |
| Accuracy            | 83.63% |
| Precision (Default) | 33.94% |
| Recall (Default)    | 39.05% |
| F1-Score (Default)  | 36.32% |
| ROC-AUC             | 0.7464 |

A threshold of 0.45 was also tested, achieving an F1-score of approximately 0.364 for the default class.

The threshold affects the balance between identifying potential defaults and generating false alarms.

## 📁 Dataset Features

The dataset includes borrower information such as:

* Age and income
* Loan amount and loan term
* Credit score
* Employment duration
* Number of credit lines
* Interest rate
* Debt-to-income ratio
* Education and employment type
* Marital status
* Mortgage and dependent information
* Loan purpose and co-signer status

**Target variable:** `Default`

* `0` — Non-Default
* `1` — Default

## ⚙️ Project Workflow

1. Load the dataset.
2. Explore and visualize the data.
3. Check missing values and duplicate records.
4. Separate input features and target variable.
5. Split data into training and testing sets.
6. Encode categorical variables and scale numerical features.
7. Train machine learning models.
8. Compare model performance.
9. Evaluate predictions using a confusion matrix and classification report.
10. Build an interactive Gradio interface.
11. Save the trained model and selected decision threshold.

## 🚀 How to Run

1. Open the project notebook in Google Colab.
2. Upload the dataset when requested.
3. Run the notebook cells in order.
4. Train the models and evaluate their performance.
5. Launch the Gradio interface.
6. Enter borrower details to receive a prediction.

Required Python libraries include:

```bash
pip install pandas numpy matplotlib scikit-learn gradio joblib
```

## ⚠️ Disclaimer

This project is developed for educational purposes. Predictions are estimates based on historical data and should not be used as the sole basis for real-world lending decisions.


