# California Housing Price Prediction Model

## Project Overview

This project builds a machine learning model to predict median house values in California based on various geographical and demographic features. The model uses a **Linear Regression** approach to establish relationships between housing features and their market prices.

## Dataset

The project uses the California Housing dataset, which contains 20,640 instances with the following features:

- **Longitude**: Geographic longitude coordinate
- **Latitude**: Geographic latitude coordinate
- **Housing Median Age**: Median age of houses in the area
- **Total Rooms**: Total number of rooms in all houses
- **Total Bedrooms**: Total number of bedrooms in all houses
- **Population**: Total population in the area
- **Households**: Number of households
- **Median Income**: Median income in the area (in units of $10,000)
- **Ocean Proximity**: Categorical feature indicating proximity to ocean (e.g., '<1H OCEAN', 'INLAND', 'ISLAND', 'NEAR BAY', 'NEAR OCEAN')
- **Median House Value**: Target variable (median house price in units of $100,000)

**Data Source**: housing.csv

## Project Structure

```
California_Housing_Price_Prediction_Model/
├── California_Housing_Prediction_Model.ipynb  # Main Jupyter notebook
├── housing.csv                                 # Dataset file
├── JPN.ipynb                                   # Additional analysis notebook
└── README.md                                   # This file
```

## Key Steps

### 1. **Data Exploration & Analysis**
   - Load dataset and examine structure
   - Generate descriptive statistics
   - Analyze correlations between features
   - Visualize geographical distribution of housing prices

### 2. **Data Preprocessing**
   - Handle missing values (particularly in 'total_bedrooms')
   - Encode categorical variables using one-hot encoding
   - Remove unnecessary categorical columns after encoding

### 3. **Feature Engineering**
   - Separate features (X) from target variable (y)
   - Prepare data for model training

### 4. **Model Training & Evaluation**
   - Split data: 80% training, 20% testing
   - Train Linear Regression model (OLS)
   - Calculate model performance metrics (R-squared, coefficients)
   - Generate predictions on test set

### 5. **Visualization & Error Analysis**
   - Plot residuals to visualize prediction errors
   - Compare actual vs. predicted values
   - Analyze model performance across observations

## Requirements

```python
numpy
pandas
matplotlib
scikit-learn
```

