# California Housing Price Prediction 🏡

## 📌 Project Overview
This project aims to predict **median house values in California** using machine learning techniques. It follows a complete end-to-end ML workflow, including data acquisition, exploratory data analysis, feature engineering, model training, and evaluation. The goal is to compare different regression models and understand how well they perform on structured housing data.

---

## 📊 Dataset
- **Source:** California Housing Dataset (via KaggleHub)
- **Target Variable:** `median_house_value`
- **Key Features:**
  - Longitude & Latitude
  - Housing median age
  - Total rooms & total bedrooms
  - Population
  - Households
  - Median income

---

## 🔍 Exploratory Data Analysis (EDA)
- Examined feature distributions and correlations
- Identified skewed numerical features
- Analyzed relationships between predictors and the target variable

---

## 🛠️ Data Preprocessing & Feature Engineering
- Applied **log transformations** to skewed features:
  - `total_rooms`
  - `total_bedrooms`
  - `population`
  - `households`
- Engineered new features:
  - **Bedroom ratio** (total_bedrooms / total_rooms)
  - **Rooms per household**
- Split data into **training and testing sets**

---

## 🤖 Models Used
The following regression models were trained and compared:

- **Linear Regression**
- **Lasso Regression (L1 Regularization)**
- **Ridge Regression (L2 Regularization)**
- **Random Forest Regressor**

---

## 📈 Evaluation Metrics
Models were evaluated using multiple regression metrics:
- R-squared (R²)
- Adjusted R-squared
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- Mean Squared Error (MSE)

Visual comparisons of **actual vs. predicted values** were also created for the linear models.

---

## 🏆 Results & Findings
- Linear models performed reasonably well after feature engineering.
- Regularization (Lasso & Ridge) helped control model complexity.
- **Random Forest Regressor achieved the best performance**, demonstrating a stronger ability to capture non-linear relationships in the data.

---

## ⚠️ Limitations
- The dataset contains an upper cap on house values, which may limit prediction accuracy for high-priced homes.
- No hyperparameter tuning or cross-validation was applied (future improvement).

---

## 🚀 Future Improvements
- Apply cross-validation
- Perform hyperparameter tuning (GridSearch / RandomizedSearch)
- Add feature importance analysis
- Try advanced models (XGBoost, Gradient Boosting)

---

## 🧰 Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📁 Project Structure
