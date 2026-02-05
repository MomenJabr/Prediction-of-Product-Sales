# 📦 Prediction of Product Sales

This repository contains a Colab Notebook that performs **exploratory data analysis and machine learning modeling** for predicting product sales based on historical sales data.

The goal of this project is to analyze key features in the dataset and build predictive models that estimate future product sales. The notebook walks through data cleaning, visualization, model training, and evaluation.

---

## 🧾 Project Overview

Predicting product sales helps businesses make strategic decisions about **inventory forecasting, resource allocation, and marketing planning**. In this project, we:

- Load and explore a historical sales dataset  
- Visualize patterns and distributions of key variables  
- Calculate summary statistics like **mean** and **median**  


This type of analysis is fundamental in retail forecasting and supply chain optimization.

In addition, we build and evaluate regression models to predict **Item_Outlet_Sales** using a full **scikit-learn pipeline** (preprocessing + modeling), including a baseline **Linear Regression** and an optimized **Random Forest** model using **GridSearchCV**.

---

## 📂 Dataset

The notebook uses a dataset that includes both numerical and categorical variables related to product attributes and sales. Typical columns may include:

- `Item_Weight`  
- `Item_Outlet_Sales`  
- Other product metadata

The target variable for prediction is:

- `Item_Outlet_Sales` → represents the total sales of a product at a specific outlet.

The remaining variables are used as input features to train machine learning models.

Make sure your dataset is in the same directory as the notebook or update the file path accordingly.

---

## 🛠️ Tools & Libraries

This project uses the following Python packages:

- 🐍 `pandas` — data manipulation and analysis  
- 📊 `matplotlib` & `seaborn` — data visualization  
- 🔢 `numpy` — numerical computations  
- 🤖 `scikit-learn` — machine learning, preprocessing pipelines, model training, and hyperparameter tuning    

---

## 📈 Key Steps (Notebook Workflow)

1. **Import Libraries**  
   Load all required packages for data handling and visualization.

2. **Load Data**  
   Read the CSV file into a DataFrame.

3. **Data Cleaning**  
   Handle missing values, correct data types, and prepare features.

4. **Data Visualization**  
   Create histograms, box plots, and summary statistics to understand data distributions.
Exploratory Data Analysis (EDA)

In addition to basic visualizations, univariate and multivariate analysis were conducted to better understand feature behavior and relationships with the target variable (Item_Outlet_Sales).

🔹 Univariate Analysis

Univariate analysis was used to examine the distribution of individual features and identify potential outliers or skewness.

Key observations:

The target variable (Item_Outlet_Sales) shows a right-skewed distribution.

Some numerical features exhibit outliers that may impact model performance.

Categorical variables show imbalance across certain categories.

🔹 Multivariate Analysis

Multivariate analysis was performed to explore relationships between features and their combined impact on sales.

Key observations:

Item_MRP shows a strong relationship with Item_Outlet_Sales.

Store-related features such as Outlet_Type and Outlet_Size appear to influence sales levels.

Some features (e.g., Item_Weight) show weak or no direct relationship with the target variable.


5. **Feature Preprocessing Pipeline**

Numerical and categorical features were preprocessed using scikit-learn pipelines:

- Missing values handled using SimpleImputer  
- Numerical features scaled using StandardScaler  
- Categorical features encoded using OneHotEncoder and OrdinalEncoder  
- ColumnTransformer used to combine preprocessing steps  

This ensures proper data preparation and prevents data leakage.


6. **Model Training**

Two regression models were trained:

- Linear Regression (baseline model)
- Random Forest Regressor (nonlinear model)

Both models were integrated into full pipelines including preprocessing.



7. **Hyperparameter Tuning**

GridSearchCV was used to optimize Random Forest parameters such as:

- n_estimators
- max_depth
- min_samples_split
- min_samples_leaf

This improved model performance.



8. **Model Evaluation**

Models were evaluated using:

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

The tuned Random Forest model achieved the best performance.

---

##  How to Run

1. Clone this repository:

```bash
https://github.com/MomenJabr/Prediction-of-Product-Sales.git
