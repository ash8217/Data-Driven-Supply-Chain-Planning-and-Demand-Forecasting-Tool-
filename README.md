# Supply Chain Optimization with Demand Forecasting

## Project Overview
This project focuses on **optimizing the supply chain** by predicting **weekly sales** for retail stores using a machine learning approach.  
We employed a **RandomForestRegressor** model trained on store attributes, promotions, and external factors to generate predictions.  
The analysis provides insights into sales drivers and supports **data-driven decisions** for inventory and supply chain operations.

## Objective
The project aims to forecast **Weekly_Sales** using historical data with features such as promotions, store type, holidays, and seasonal effects.  
Key goals include:
- Delivering accurate sales predictions for **inventory management**.  
- Evaluating feature importance to identify sales drivers.  
- Visualizing sales patterns and performance metrics to extract insights.  

## Dataset
The project uses four datasets:  
- **Features.csv** – Promotional events and weather data.  
- **Stores.csv** – Store information, including type and assortment.  
- **Train.csv** – Historical weekly sales data for model training.  
- **Test.csv** – Data for evaluating model performance.  

## Step-by-Step Process

### Step 1: Data Loading
- Loaded datasets with **Pandas**.  
- Merged features, stores, and train datasets into a unified dataset with all store-level information.  

### Step 2: Data Preprocessing
- **Merging Datasets** – Combined features, stores, and train data.  
- **Handling Missing Values** – Numeric columns filled with median, categorical with mode.  
- **Feature Engineering** – Extracted Year, Month, Week, Day, and DayOfWeek from the Date column.  
- **Encoding Categorical Variables** – Applied one-hot encoding to prepare data for ML models.  

### Step 3: Model Training
- Trained **RandomForestRegressor** to predict `Weekly_Sales` using processed features.  

### Step 4: Model Evaluation
- **Mean Squared Error (MSE):** Measured average squared error between actual and predicted sales.  
- **R-squared (R²):** Evaluated variance explained by the model.  

### Step 5: Feature Importance Analysis
- Plotted **top 10 features** impacting predictions, highlighting the strongest sales drivers.  

### Step 6: Visualizations
Using **Plotly** and other libraries, created:  
- **Sales Trend Over Time** – Line plot of Weekly_Sales to observe seasonal trends.  
- **Sales Distribution by Store Type** – Boxplot comparing sales across store types.  

## Tools and Technologies
- **Python** – Core language for analysis and modeling.  
- **Pandas** – Data manipulation and preprocessing.  
- **Scikit-Learn** – Machine learning model training and evaluation.  
- **Seaborn & Plotly** – Visualization and interactive insights.  
- **Matplotlib** – Standard plotting support.  

