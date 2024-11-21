Overview 
This project focuses on analyzing and building a machine learning pipeline for a user behavior classification dataset. The goal is to clean the data, explore its structure, engineer 
relevant features, and evaluate various regression models to predict the target variable, User Behavior Class.

Features
Data Cleaning

Handling missing values.
Outlier detection and treatment using the IQR method.
Dropping irrelevant columns (e.g., User ID).
Data Visualization

Box plots for outlier analysis.
KDE plots for distribution comparison.
Pie charts for categorical feature distributions.
Feature Engineering

Creating derived features like weekly app usage and app usage to screen time ratio.
Binning features into categories (e.g., number of apps installed).
Feature Selection

Using SelectKBest to select the top features for modeling.
Modeling

Evaluating multiple regression algorithms:
Linear Regression
Random Forest Regressor
Gradient Boosting Regressor
SVR, and more.
Hyperparameter tuning using Grid Search.
Saving the best model using pickle.
Data Cleaning and Visualization
Missing Values
Checked for missing values in each column and handled them by either imputing or removing rows.

Outlier Detection
Used box plots and the IQR method to detect and handle outliers in numerical columns.

Visualizations
KDE Plots: To explore distributions for app usage and other metrics.
Pie Charts: To analyze the distribution of categorical features like operating system, device model, and gender.
Feature Engineering
New Features
App Usage Total (week): Calculated as daily app usage multiplied by 7.
App Usage to Screen Time Ratio: Created a feature to represent user engagement with apps relative to their screen time.
Feature Binning
Categorized continuous variables like the number of apps installed into Low, Medium, and High.

Modeling
Algorithms Evaluated
Linear Regression
SGD Regressor
Lasso, Ridge
Random Forest Regressor
Gradient Boosting Regressor
SVR
Decision Tree Regressor
KNN Regressor
Model Selection
Performed Grid Search to find the best hyperparameters for each model.
Selected the model with the lowest Mean Squared Error (MSE) as the final model.
Saved the best model as best_model.sav using pickle.
