# Traffic Accident Data Analysis (Python)

Data cleaning, visualization and correlation analysis of a traffic accident dataset using Python.

## Overview
Group project for MDA3003 Introduction to Data Science, Universiti Malaysia Terengganu. The project explores factors that may influence traffic accident occurrence and prepares the data for future predictive modelling.

## Dataset
840 records and 14 attributes covering weather, road type, time of day, traffic density, speed limit, number of vehicles, driver age and experience, driver alcohol use, accident severity, road and light conditions, and the target variable `Accident` (0 = no, 1 = yes). In the cleaned data, 239 records are accidents and 601 are not, so the target is imbalanced.

## What was done
1. Inspected the data and detected 588 missing values (42 per column), visualised with a heatmap
2. Filled missing values with the most frequent value of each column
3. Saved the cleaned dataset
4. Explored distributions with box plots and relationships with bar plots
5. Analysed correlations between attributes and the target

## Key findings
- Driver age and driver experience are strongly related, so using both in a model may be redundant
- Road type and speed limit are related (highways have higher speed limits)
- Road condition, light condition, weather and traffic density showed weak correlation with accident occurrence
- The imbalanced target would need oversampling or undersampling before modelling

## Files
- `Group_5.ipynb`: Jupyter Notebook with the full analysis
- `dataset_traffic_accident_prediction.csv`: original dataset
- `cleaned_dataset_traffic_accident_prediction.csv`: dataset after cleaning

## Tools
Python, pandas, seaborn, matplotlib, scikit-learn, Jupyter Notebook
