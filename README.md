# Ecommerce Customer Data Analysis and Linear Regression

This repository contains a data analysis and machine learning model for customer data from an e-commerce company. The analysis includes data preprocessing, outlier detection, and a linear regression model to predict yearly spending by customers.

## Overview

- **Data Source:** The dataset used in this analysis is named 'Ecommerce Customers.csv'. It contains customer information, including their session length, time spent on the app, time spent on the website, length of membership, and yearly amount spent.

- **Analysis Steps:** The project involves the following steps:

    1. **Data Preprocessing**: We start by importing necessary libraries, loading the dataset, and dropping irrelevant columns (Email, Address, Avatar).
    
    2. **Data Visualization**: We use Plotly Express to create box plots for key features and detect and remove outliers in the dataset.
    
    3. **Data Modeling**: The data is split into training and testing sets, features are standardized, and a linear regression model is created. The model's training and testing scores are evaluated.


