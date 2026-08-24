# Predictive Modeling and Optimization for Logistics Operations

## Project Overview

This project applies predictive modeling and optimization techniques to a logistics delivery-time forecasting problem.

A simulated dataset containing 1,500 shipment records was created using Python. The project analyzes operational factors such as distance, traffic, weather, package weight, vehicle type, driver experience, stop count, and peak-hour conditions.

The objective is to predict delivery time and use predictive insights to improve logistics operations.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Machine Learning Models

The following regression models were developed and evaluated:

1. Linear Regression
2. Random Forest Regression

## Evaluation Metrics

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

## Model Results

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 6.22 | 7.60 | 0.9579 |
| Random Forest | 9.45 | 11.87 | 0.8972 |

Linear Regression achieved the best performance on the executed test dataset.

## Cross-Validation

Five-fold cross-validation was performed for the Random Forest model.

Average Cross-Validation MAE:

9.71 minutes

## Hyperparameter Tuning

GridSearchCV was used to tune the Random Forest model.

Best parameters:

- n_estimators = 200
- max_depth = 20
- min_samples_leaf = 1

## Feature Importance

Distance_KM was the most important feature with an importance of approximately 0.6999.

Stop_Count was the second most important feature with an importance of approximately 0.1209.

## Delay-Risk Analysis

Shipments with predicted delivery time greater than 100 minutes were classified as High Risk.

Among the 300 test shipments:

- High Risk: 196
- Normal: 104

## Optimization Strategies

The project proposes the following logistics optimization strategies:

- Dynamic driver allocation
- Traffic-aware scheduling
- Route prioritization
- Vehicle matching
- Stop consolidation
- Proactive customer communication
- Resource planning

## Project Files

- `Logistics_Predictive_Modeling_Optimization.ipynb` - Complete Google Colab notebook
- `logistics_delivery_dataset.csv` - Simulated logistics dataset
- `Logistics_Predictive_Modeling_Optimization_Report.docx` - Detailed technical report

## Conclusion

The project demonstrates an end-to-end machine-learning workflow for logistics delivery-time prediction and operational optimization.

Although the dataset is simulated, the methodology can be extended to real-world logistics data containing GPS, traffic, weather, vehicle, driver, and historical delivery information.
