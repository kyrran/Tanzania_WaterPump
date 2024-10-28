# Failing Water Points in Tanzania: Predictive Analysis for Human-Powered Pumps

## Project Overview
This project explores the factors affecting the functionality of human-powered water pumps in Tanzania, using machine learning models to predict pump failure based on population density and management type. The project aims to support water management in Tanzania by identifying key factors that could guide better maintenance and resource allocation.

This project is built upon the [Pump It Up: Data Mining the Water Table](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/) competition by DrivenData, focused on predicting the functionality of water points in Tanzania to improve resource allocation and water accessibility.

## Dataset
The analysis uses data from Taarifa’s waterpoint dashboard, encompassing 59,401 entries with various features related to the water points' operational status, population density, and management. 

## Objectives
1. **Population Impact**: Determine if pumps in regions with high population density are more likely to fail than those in low-density regions.
2. **Management Type Impact**: Assess if locally managed pumps have a higher likelihood of failure compared to state-managed ones.

## Methodology
- **Data Preprocessing**: Cleaned and preprocessed the dataset, reducing noise and irrelevant columns. Addressed missing values and encoded categorical variables to prepare for model training.
- **Feature Selection**: Applied Random Forest and correlation analysis to select relevant features, refining the data for enhanced model accuracy.
- **Modeling Techniques**: 
  - Implemented and tuned **K-Nearest Neighbors (KNN)**, **Support Vector Machines (SVM)**, and **Random Forest** classifiers.
  - **Evaluation Metrics**: Accuracy, Precision, and Recall were used to assess model performance, with SVM achieving the highest accuracy of 71.2% for population-based predictions and Random Forest performing best for management-based analysis.

## Results
- **Population Analysis**: SVM achieved a 71.2% accuracy, indicating a correlation between higher population regions and pump failure rates.
- **Management Analysis**: Random Forest provided reliable predictions on management effectiveness, suggesting state-managed pumps are generally more reliable than locally managed ones.
  
## Key Findings
- Pumps in low population areas tend to have higher failure rates, potentially due to limited maintenance resources.
- State-managed water points demonstrated higher functionality rates than locally managed ones, underscoring the importance of management quality in pump reliability.

## Future Work
- **Feature Expansion**: Explore additional features, such as geographical factors, to improve model predictions.
- **Model Tuning**: Further refine model hyperparameters and feature selection for increased accuracy.
- **Broader Application**: Extend the analysis to motor-powered pumps and assess the impact of different maintenance strategies.

## Dependencies
- **Python 3.7+**
- Libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`

## Contributors
- **Kangle Yuan** - Feature engineering, SVM and Random Forest modeling, data analysis
- **Abinaya Maruthalingam** - Data preprocessing, KNN and SVM modeling, report formatting
