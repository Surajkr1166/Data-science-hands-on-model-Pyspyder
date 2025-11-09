📘 README.md — Loan Default Prediction using PCA and Logistic Regression
🧠 Project Overview

This project aims to predict loan default using Logistic Regression enhanced with Principal Component Analysis (PCA) for dimensionality reduction.
The objective is to build a robust and interpretable machine learning model that helps financial institutions assess credit risk and improve lending decisions.

🎯 Objective

Analyze and preprocess customer data.

Use PCA to reduce feature dimensionality while preserving key information.

Apply Logistic Regression for binary classification (Default = 1, Not Default = 0).

Evaluate model performance using confusion matrix, ROC curve, and AUC score.

⚙️ Tech Stack

Language: Python 🐍

Environment: Google Colab / Jupyter Notebook

Libraries Used:

pandas, numpy, matplotlib, seaborn, sklearn

📊 Project Workflow
1️⃣ Data Preprocessing

Import dataset containing financial and demographic features.

Handle missing values and outliers.

Encode categorical variables.

Standardize features using:

from sklearn.preprocessing import StandardScaler

2️⃣ Dimensionality Reduction using PCA

Why PCA?
PCA helps simplify the dataset by transforming correlated features into uncorrelated principal components, making the model faster and reducing noise.

Steps:

from sklearn.decomposition import PCA


Standardize data.

Apply PCA to extract the top components that explain the majority of variance.

Choose components with cumulative variance > 90%.

Visualize explained variance ratio.

Output:

New reduced dataset with fewer features but maximum information retained.

Easier visualization and improved model performance.

3️⃣ Logistic Regression Model

Apply Logistic Regression on PCA-transformed data:

from sklearn.linear_model import LogisticRegression


Fit the model to the training data and predict loan default probabilities.

4️⃣ Model Evaluation

Evaluate using classification metrics:

Metric	Description
Accuracy	Measures correct predictions
Precision	How many predicted defaults were correct
Recall (Sensitivity)	How many actual defaults were caught
F1 Score	Balance between precision and recall
ROC & AUC	Measure overall separability and performance

Visualization:

from sklearn.metrics import confusion_matrix, roc_curve, auc, accuracy_score

📈 5️⃣ Visualizations

Explained Variance Plot (to choose PCA components)

ROC Curve for classification performance

Confusion Matrix Heatmap for result interpretation

🧾 Conclusion

PCA effectively reduced data dimensionality while keeping key patterns.

Logistic Regression on PCA-transformed data gave high interpretability and stable accuracy.

AUC Score close to 1 indicates strong predictive power.

🔹 Future Scope:

Try Regularization (L1/L2) to avoid overfitting.

Compare results with Ensemble methods like Random Forest or XGBoost.

Perform Hyperparameter tuning using GridSearchCV.
