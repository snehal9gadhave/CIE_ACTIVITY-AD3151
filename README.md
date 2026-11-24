# Multiple Linear Regression – CIE 2 Activity

**Roll Number:** AD3151  
**Subject:** Regression and Classification Algorithms  
**Dataset:** Weather Dataset  
**Target Variable:** MaxTemp  
**Programming Language:** Python  
**Platform:** Google Colab / Jupyter Notebook  

## 1. Introduction
Multiple Linear Regression is a supervised machine learning algorithm used to predict a continuous value using two or more independent variables.

In this activity, a Weather Dataset is used to predict maximum temperature (MaxTemp) using different weather-related features. The main aim is to understand how multiple input features affect the target variable and compare single-feature and multiple-feature regression models.

## 2. Dataset Description
- **Dataset File:** weather(2).csv
- **Total Rows:** 366
- **Total Columns:** 22
- **Input Features:** MinTemp, Sunshine, Humidity3pm, Pressure3pm, Cloud3pm and WindSpeed3pm.
- **Target Variable:** MaxTemp (°C)
- **Dataset Source:** Add the original dataset source link here.

The dataset contains information about different weather conditions. These features are selected because they may influence the maximum temperature.

## 3. Objectives
- To understand Multiple Linear Regression.
- To perform manual least-squares calculations.
- To build Single and Multiple Linear Regression models.
- To interpret regression coefficients.
- To check correlation and multicollinearity.
- To evaluate model performance using different metrics.
- To predict maximum temperature for a new record.

## 4. Data Preprocessing and EDA
The dataset is loaded using Pandas and inspected to understand its structure.

The following operations are performed:
- Display first five records.
- Check rows, columns and data types.
- Calculate summary statistics.
- Identify and handle missing values.
- Check duplicate records.
- Create scatter plots and correlation heatmap.

The visualisations help understand relationships between the input features and maximum temperature.

## 5. Manual Calculation
Manual Multiple Linear Regression is performed using six observations and two input features:

- X1 = MinTemp
- X2 = Sunshine
- y = MaxTemp

The design matrix, target vector, XTX and XTy are calculated.

The normal equation is:

**b = (XᵀX)⁻¹Xᵀy**

The coefficients b0, b1 and b2 are calculated and used to form the regression equation. The manual results are verified using Scikit-learn.

## 6. Model Building
The dataset is divided into training and testing sets using an 80:20 split.

Two models are developed:

**Single Linear Regression:** Uses one input feature to predict maximum temperature.

**Multiple Linear Regression:** Uses all six selected input features to predict maximum temperature.

The models are trained using the training data and evaluated using unseen test data.

## 7. Model Evaluation
The following evaluation metrics are calculated:

- **MAE:** Measures average absolute prediction error.
- **MSE:** Measures average squared prediction error.
- **RMSE:** Measures prediction error in the target's unit.
- **R² Score:** Measures how well the model explains target variation.
- **Adjusted R²:** Evaluates model performance while considering the number of features.

A comparison table is created to check whether multiple features improve prediction performance.

## 8. Visualisation and Multicollinearity
The following graphs and checks are performed:

- Correlation Heatmap
- Residual Plot
- Residual Histogram
- Actual vs Predicted Plot
- VIF (Variance Inflation Factor)

These analyses help identify relationships among features, prediction errors and possible multicollinearity.

## 9. New Prediction
A new weather record is given to the trained Multiple Linear Regression model.

The model predicts the maximum temperature using the selected input features. The prediction is checked against the training-data ranges to avoid unsupported extrapolation.

**Predicted MaxTemp:** Add the actual notebook output here (°C).

## 10. Conclusion
In this activity, Multiple Linear Regression is used to predict maximum temperature using different weather-related features.

Manual calculations are performed and verified using Python libraries. Single-feature and multiple-feature models are compared using evaluation metrics.

Correlation, VIF and residual analysis are used to understand model performance and limitations.

The activity demonstrates that adding more features does not always improve prediction accuracy. The best model should be selected based on its performance on unseen data.

## 11. Project Files
- `Weather_Multiple_Linear_Regression_Activity.ipynb` – Executed notebook with code and outputs.
- `weather(2).csv` – Dataset used for the activity, if redistribution is permitted.
- `README.md` – Project description and methodology.
- `Activity_Report.pdf` – Activity report, if included.

## 12. Faculty GitHub Reference
Submission GitHub ID: [complexiota](https://github.com/complexiota)

## 13. Student Details
**Roll Number:** AD3151  
**Repository Name:** CIE_AD3151
