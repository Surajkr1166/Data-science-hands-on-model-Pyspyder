📘 README.md — Logistic Regression Loan Default Prediction
🧠 Project Overview

This project applies Logistic Regression to predict whether a customer will default on a loan or not.
The main goal is to build a binary classification model that helps financial institutions make better lending decisions and reduce risk.

🎯 Objective

To analyze customer financial data.

To classify loan applicants as “Default” (1) or “Not Default” (0).

To evaluate model performance using metrics like accuracy, confusion matrix, ROC curve, and AUC.

⚙️ Tech Stack

Language: Python 🐍

Environment: Jupyter Notebook (.ipynb)

Libraries Used:

pandas, numpy, matplotlib, seaborn, sklearn

📊 Project Workflow
1️⃣ Data Collection

Dataset contains customer demographic and financial information.

Target variable → loan_default (1 = Default, 0 = No Default).

2️⃣ Data Preprocessing

Handling missing values.

Encoding categorical features.

Feature scaling for logistic regression.

Splitting data into train and test sets.

3️⃣ Model Building

Implemented Logistic Regression using:

from sklearn.linear_model import LogisticRegression


Trained the model on training data and predicted on test data.

4️⃣ Model Evaluation

Confusion Matrix: To measure true/false positives and negatives.

Accuracy Score: Overall model correctness.

ROC Curve & AUC: To visualize performance and check model’s ability to separate classes.

from sklearn.metrics import roc_curve, auc, confusion_matrix, accuracy_score

5️⃣ Insights

Higher AUC indicates a strong ability to distinguish between default and non-default cases.

Logistic regression provides interpretable coefficients showing feature importance.

📈 Evaluation Metrics
Metric	Description
Accuracy	Overall correctness of predictions
Precision	How many predicted defaults were correct
Recall (Sensitivity)	How many actual defaults were detected
AUC-ROC	Model’s ability to separate classes visually and numerically
🧩 Visualization

Correlation heatmap for feature analysis.

ROC Curve to visualize trade-off between TPR and FPR.

Confusion matrix plot for prediction summary.

🧾 Conclusion

Logistic Regression effectively predicts loan default probability.

The model is interpretable and useful for financial decision-making.

Future improvements:

Try ensemble methods like Random Forest or XGBoost.

Feature engineering to improve predictive power.
