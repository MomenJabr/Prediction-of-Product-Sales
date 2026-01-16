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

---

## 📂 Dataset

The notebook uses a dataset that includes both numerical and categorical variables related to product attributes and sales. Typical columns may include:

- `Item_Weight`  
- `Item_Outlet_Sales`  
- Other product metadata

Make sure your dataset is in the same directory as the notebook or update the file path accordingly.

---

## 🛠️ Tools & Libraries

This project uses the following Python packages:

- 🐍 `pandas` — data manipulation and analysis  
- 📊 `matplotlib` & `seaborn` — data visualization  

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



---

##  How to Run

1. Clone this repository:

```bash
https://github.com/MomenJabr/Prediction-of-Product-Sales.git
