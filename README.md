# What Drives the Price of a Car?

## Project Overview

This project analyzes a used-car dataset to determine which vehicle characteristics are most strongly associated with listing price. The analysis follows the CRISP-DM framework and is written for a used-car dealership interested in improving inventory purchasing and pricing decisions.

## Business Question

Which vehicle characteristics have the greatest influence on used-car listing prices, and how can a dealership use these insights to make better pricing and inventory decisions?

## Dataset

The analysis uses a reduced version of the Kaggle used-car dataset containing vehicle characteristics such as:

- Manufacturer
- Model
- Vehicle age
- Odometer
- Fuel type
- Transmission
- Vehicle type
- Condition
- Listing price

## Methodology

The project follows the CRISP-DM process:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Exploratory Data Analysis
5. Modeling
6. Evaluation
7. Recommendations

The models evaluated include:

- Linear Regression
- Ridge Regression
- Linear Regression with a log-transformed target
- Ridge Regression with a log-transformed target

Five-fold cross-validation and GridSearchCV were used to evaluate model stability and tune the Ridge regularization parameter.

## Main Findings

- Newer vehicles generally have higher listing prices.
- Higher mileage is associated with lower listing prices.
- Manufacturer, vehicle type, fuel type, and transmission are also associated with price differences.
- Trucks and pickups have relatively high average listing prices.
- The best-performing model was Ridge Regression with a log-transformed target.

## Model Performance

The final model achieved:

- MAE: approximately $3,642
- RMSE: approximately $6,505
- R²: 0.7795

The model explained approximately 78% of the variation in used-car listing prices.

## Business Recommendations

- Prioritize newer, lower-mileage vehicles when purchasing inventory.
- Consider manufacturer and vehicle type when setting acquisition budgets.
- Use the model as a pricing-support tool rather than as the sole pricing decision.
- Manually review predictions for unusual, luxury, or highly customized vehicles.
- Retrain the model periodically as market conditions change.


## Notebook

View the complete analysis here:

[Assignment 11.1 - Used Car Price Analysis](Assignment_11_1_Used_car_price_analysis.ipynb)

