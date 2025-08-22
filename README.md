# Used Car Condition and Price Prediction

## Introduction
This project, completed as part of an **Estarta Intern** task, focuses on predicting **used car conditions** and **market prices** using real-world data. It aims to help buyers, sellers, and dealers make informed decisions by leveraging machine learning models.

## Dataset
The dataset contains **380,180 records** with **26 attributes** such as `price`, `year`, `manufacturer`, `model`, `odometer`, `condition`, and more. It is real-world data, reflecting actual listings, which makes the predictions practical and relevant.

## Data Cleaning and Preprocessing
- Handled missing values by removing columns with excessive missing data and filling or labeling other missing entries.
- Removed very extreme outliers in `price`, `odometer`, and `year`.
- Checked for duplicates (none found).
- Created a new feature: **Car Age** (`Current Year - Year of Manufacture`).

## Data Exploration
- Visualized key patterns in the dataset, such as:
  - Top 15 car manufacturers by count
  - Average price by top manufacturers
  - Price vs. odometer (sample of 1,000)
  - 
## Simple Feature Engineering 
  - car age

## Classification: Car Condition
- Target variable: `condition` (categories: Excellent, Good, Fair, Poor)
- Models used:
  - **Decision Tree**: 89% accuracy
  - **XGBoost**: 95% accuracy
- Categorical features and target were encoded; dataset was split into training/testing sets.
- Confusion matrix visualizations included in the report.

## Regression: Predicting Car Price
- Models used:
  - **XGBoost**
    - MAE: 3,345.72
    - RMSE: 5,607.85
    - R²: 0.845
  - **Random Forest**
    - MAE: 2,004.46
    - RMSE: 4,524.44
    - R²: 0.899
- Feature importance analyzed and visualized.
- Linear regression models were tested but performed poorly due to non-linear relationships.

## Conclusion
- Tree-based models (Decision Tree, XGBoost, Random Forest) are effective for predicting car condition and price.
- The project provides practical insights for the used car market.
- Feature importance highlights key drivers: car age, odometer, manufacturer, and condition.
