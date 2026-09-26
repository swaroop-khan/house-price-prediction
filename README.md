# 🏠 House Price Prediction

An end-to-end machine learning project for the Kaggle House Prices: Advanced Regression Techniques competition.

## 🎯 Objective

Predict residential house sale prices using features such as:

- Overall quality
- Living area
- Neighborhood
- Year built
- Garage and basement features
- Other property characteristics

## 🔍 Approach

EDA → Missing Value Analysis → Feature Analysis → Data Preprocessing → Model Comparison → Hyperparameter Tuning → 5-Fold Cross-Validation → Final Prediction → Kaggle Submission

## 🤖 Models & Results

| Model | RMSLE |
|---|---:|
| Raw Linear Regression | 0.1782 |
| Log-Target Linear Regression | 0.1416 |
| Random Forest | 0.1458 |
| **Gradient Boosting** | **0.1338** |

### Final Gradient Boosting Model

The final model used:

- `n_estimators = 300`
- `learning_rate = 0.05`
- `max_depth = 3`

The target variable was log-transformed using `log1p` to reduce the effect of its skewed distribution.

## 📊 Validation

5-Fold Cross-Validation:

- Mean RMSLE: **0.13135**
- Standard Deviation: **0.02170**

## 🏆 Kaggle Result

The final model was trained on the complete training dataset and used to generate predictions for the Kaggle test set.

**Kaggle RMSLE: 0.13342**

The submission file contains:

- `Id`
- `SalePrice`

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Git & GitHub
- Kaggle

## 📁 Project Structure

    house-price-prediction/
    ├── 01_house_price_eda.ipynb
    ├── submission.csv
    ├── .gitignore
    └── README.md

The Kaggle dataset and Python virtual environment are excluded from the repository.

## 🧠 Key Learnings

- Exploratory Data Analysis
- Missing-value handling
- Numerical and categorical preprocessing
- Log transformation
- Gradient Boosting
- Hyperparameter tuning
- Holdout validation
- 5-fold cross-validation
- RMSLE evaluation
- Kaggle submissions
- Git & GitHub

## 🔗 Competition

[Kaggle — House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

**Kaggle Leaderboard RMSLE:** 0.13342
