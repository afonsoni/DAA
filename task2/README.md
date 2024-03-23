## Task 2 - Competition Dataset Task

## Solar Energy Prediction - Machine Learning Competition

### Introduction

This project analysis and development of Machine Learning models for a solar energy prediction competition. The main goal was to predict the amount of solar energy injected into the power grid every hour of the day, using historical data on energy consumption and production, along with weather and geographical information.

### Data Acquisition and Preprocessing

1. **Datasets:**

- Weather Data: Divided into three periods (September 2021 to December 2021, January 2022 to December 2022, and January 2023 to April 2023).
- Energy Consumption Data: Corresponding to the weather data periods.
- OpenMeteo Weather Data: Complements the available weather data, focusing on relevant analysis variables.

2. **Preprocessing:**

- Identification of missing values and treatment with heatmaps.
- Conversion of the 'dt_iso' column to date and time format.
- Creation of 'date' and 'hour' columns.
- Reordering of datasets.
- Removal of unnecessary columns ('sea level', 'grnd level', 'city name', and 'weather description').
- Replacement of missing values in 'rain_1h' with zero.

### Exploratory Analysis

- Descriptive statistics of the datasets.
- Visualization of correlations between variables.
- Identification of patterns and outliers.

### Machine Learning Models

- Decision Tree Classifier:
    - Baseline model without hyperparameter tuning (accuracy of 86.2%).
    - Hyperparameter optimization with Grid Search (accuracy of 87.5%).
    - Maximum depth optimization (accuracy of 88.11%).
    - Cost-Complexity Pruning (accuracy of 87.13%).
- Bagging Classifier:
    - Decision Tree as base (accuracy of 88.36%).
- Random Forest Classifier:
    - Tuned hyperparameters (accuracy of 88.52%).
- Gradient Boosting Classifier:
    - Accuracy of 84.68%.
- Stacking Classifier:
    - Decision Tree and Random Forest as estimators.
    - Logistic Regression as final estimator (accuracy of 88.72%).

### Results and Competition Ranking

- Score of 0.87341 on the Kaggle platform.
- 17th position among 52 participating teams.

### Potential Improvements

- Exploration of other Machine Learning algorithms.
- Fine-tuning of hyperparameters.
- Acquisition of more data.
- More sophisticated handling of missing values.
- Feature selection.
- Ensemble learning with other techniques.

### Conclusion

Developing Machine Learning models for solar energy prediction is an ongoing process that can be improved by exploring new techniques, fine-tuning parameters, and increasing the quantity and quality of data. Implementing the improvements mentioned above can lead to even better results in the competition and contribute to research advancements in this field.

### Resources

- **Kaggle Competition:** [Competition](https://www.kaggle.com/c/daasbstp2023)
- **Code:** [Python Notebook](EDA.ipynb)