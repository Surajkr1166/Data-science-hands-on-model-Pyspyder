# Data-science-hands-on-model-Linear Regression 
🏠 Housing Price Prediction Using Multiple Linear Regression
📘 Project Overview

This project focuses on predicting housing prices in the Delhi region using a Multiple Linear Regression model. The objective is to understand and quantify how various features — such as area, number of bedrooms, bathrooms, and amenities — affect property prices.

By analyzing the dataset and building a regression model, the project provides a data-driven approach to price optimization for a real estate company.

🎯 Objectives

Identify the key variables influencing property prices (e.g., area, rooms, stories, parking).

Develop a linear regression model that relates these variables to property prices.

Evaluate model performance and interpret how each feature impacts pricing decisions.

🧠 Methodology
1. Data Understanding

The dataset (Housing.csv) contains 545 records and 13 columns, including both numerical and categorical features.
Key attributes include:

price: Price of the property (target variable)

area, bedrooms, bathrooms, stories, parking: Numerical predictors

mainroad, guestroom, basement, airconditioning, prefarea, furnishingstatus: Categorical predictors

2. Data Preprocessing

Handled categorical variables by mapping binary features (yes/no) to 1/0.

Used dummy encoding for multi-class variables like furnishingstatus.

Dropped redundant columns after encoding.

Checked correlations and multicollinearity using a heatmap and descriptive statistics.

3. Feature Scaling

Applied StandardScaler (from sklearn.preprocessing) to normalize numerical features, ensuring all variables were on a comparable scale.

4. Model Development

Split dataset into training (70%) and testing (30%) sets.

Trained a Multiple Linear Regression model using sklearn.linear_model.LinearRegression.

Extracted model coefficients and intercept to interpret variable impacts.

5. Model Evaluation

Predicted prices on the test set.

Evaluated model fit using metrics like:

Mean Squared Error (MSE)

R² Score (if computed)

Visualized relationships between features and price using Matplotlib and Seaborn.

🧩 Technologies Used

Python 3

Pandas – Data manipulation and preprocessing

NumPy – Numerical operations

Matplotlib / Seaborn – Visualization

Scikit-learn – Machine learning (scaling, splitting, regression model)

📊 Insights

Area showed the strongest positive correlation with price.

Houses with air conditioning, basement, or guest rooms tend to have higher prices.

Proper feature scaling significantly improved model interpretability and consistency.

📈 Future Enhancements

Implement Regularization (Lasso/Ridge Regression) to handle multicollinearity.

Add feature selection techniques to improve prediction accuracy.

Experiment with non-linear models like Decision Trees or Random Forest for comparison.
Housing.csv	The dataset used for model training and testing
Housing_Price_Prediction.ipynb	The main Jupyter Notebook containing data exploration, preprocessing, visualization, and model building code
README.md	Project documentation (this file)
