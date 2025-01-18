**1. Electricity Consumption Forecasting**

---

**Project Overview**  
This project aims to:  
- Predict electricity demand using historical consumption data and weather conditions.  
- Enable effective energy management by reducing wastage and ensuring grid stability.

---

**Dataset**  
- **Electricity Data**: Records of electricity demand and day-ahead demand forecasts.  
- **Weather Data**: Includes temperature, humidity, wind speed, dew point, and other weather-related variables.  
- Merged both datasets on a common timestamp for alignment.  

---

**Objective**  
The project goals include:  
- Exploring and preprocessing the datasets for analysis.  
- Engineering features to capture temporal and weather patterns.  
- Building and evaluating a machine learning model for electricity demand forecasting.  
- Providing actionable insights for better energy management.  

---

**Project Workflow**  
1. Data Collection and Loading:  
   - Merged electricity demand and weather data into a single dataset.  

2. Data Preprocessing:  
   - Removed irrelevant columns and handled missing values.  
   - Tested two approaches for handling missing data:  
     - Dropping rows with missing values.  
     - Imputing missing values using mean/mode for numerical and categorical features.  

3. Feature Engineering:  
   - Extracted temporal features such as year, month, day, day of the week, and weekend indicators.  
   - Selected key weather variables (e.g., temperature, humidity, wind speed) for analysis.  

4. Exploratory Data Analysis (EDA):  
   - Visualized electricity demand trends over time.  
   - Analyzed correlations between features and electricity demand using heatmaps.  

5. Modeling:  
   - Implemented a Random Forest Regressor for forecasting.  
   - Split data into training and testing sets (80-20 split).  

6. Evaluation:  
   - Assessed model performance using:  
     - RMSE (Root Mean Square Error).  
     - MAE (Mean Absolute Error).  
     - R² Score.

---

**Results**
- Method 1 (Dropping Null Values):  
  - RMSE: 6,196.02  
  - MAE: 3,887.18  
  - R² Score: 0.79  
- Method 2 (Imputing Null Values):  
  - RMSE: 7,542.66  
  - MAE: 4,504.52  
  - R² Score: 0.65  
- Dropping rows with missing values yielded better performance, highlighting the importance of data quality.  

---

**Tools and Technologies**
- Programming Language: Python  
- Libraries:  
  - Data Analysis: Pandas, NumPy  
  - Visualization: Matplotlib, Seaborn  
  - Machine Learning: scikit-learn  

---

# 2. House-Price-Prediction
Project Overview
This project focuses on:

 Predicting house prices using machine learning techniques.
 Supporting better decision-making in real estate investments and property valuation.
---

Dataset

  King County House Sales Data:

   Contains 21,613 records with features such as square footage, number of bedrooms, bathrooms, and location.
   Covers various property attributes critical for price determination.

---

**Objective**
The project goals include:

   Performing exploratory data analysis to uncover insights.
   Cleaning and preprocessing the dataset to ensure data quality.
   Building and evaluating a machine learning model to predict house prices.
   Identifying key factors influencing housing costs.

---

**Project Workflow**

  1. Data Collection and Loading:  
   - Utilized the King County dataset containing property features and prices.  

2. Data Preprocessing:  
   - Dropped irrelevant columns and handled missing values in critical features like bedrooms and bathrooms.  
   - Converted the `date` column to datetime format for enhanced analysis.  

3. Feature Engineering:  
   - Retained impactful features like square footage, bedrooms, and bathrooms.  
   - Extracted temporal information from the `date` column.  

4. Exploratory Data Analysis (EDA):  
   - Visualized relationships between house prices and key features using scatter plots.  
   - Created a correlation heatmap to identify significant predictors of price.  

5. Modeling:  
   - Implemented a Random Forest Regressor to predict house prices.  
   - Split data into training and testing sets (80-20 split).  

6. Evaluation:  
   - Assessed model performance using metrics:  
     - Mean Squared Error (MSE): 21,351,347,796  
     - R² Score: 0.86  

---

**Results**

- Achieved an R² score of 0.86, demonstrating strong predictive power.  
- Identified key features such as square footage and number of bedrooms as the most influential factors in determining house prices. 

---

**Tools and Technologies**

- Programming Language: Python  
- Libraries:  
  - Data Analysis: Pandas, NumPy  
  - Visualization: Matplotlib, Seaborn  
  - Machine Learning: scikit-learn  
