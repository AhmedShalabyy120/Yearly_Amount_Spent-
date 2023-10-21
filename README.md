# Ecommerce Customer Data Analysis and Linear Regression

This repository contains a data analysis and machine learning model for customer data from an e-commerce company. The analysis includes data preprocessing, outlier detection, and a linear regression model to predict yearly spending by customers.

## Overview

- **Data Source:** The dataset used in this analysis is named 'Ecommerce Customers.csv'. It contains customer information, including their session length, time spent on the app, time spent on the website, length of membership, and yearly amount spent.

- **Analysis Steps:** The project involves the following steps:

    1. **Data Preprocessing**: We start by importing necessary libraries, loading the dataset, and dropping irrelevant columns (Email, Address, Avatar).
    
    2. **Data Visualization**: We use Plotly Express to create box plots for key features and detect and remove outliers in the dataset.
    
    3. **Data Modeling**: The data is split into training and testing sets, features are standardized, and a linear regression model is created. The model's training and testing scores are evaluated.

## Code

The project's Python code is included in the `analysis.py` script. The code is organized into the following sections:

```python
import pandas as pd
import seaborn as sns
from sklearn.preprocessing import StandardScaler
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
import joblib
import warnings
import plotly.express as px
from datasist.structdata import detect_outliers

# ... (code for data loading and preprocessing) ...

# ... (code for data visualization and outlier removal) ...

# ... (code for data modeling and training/testing the model) ...

# Save the model, scaler, and feature list for future use
joblib.dump(model, "model.h5")
joblib.dump(scaler, "scaler.h5")
joblib.dump(features, "features.h5")
