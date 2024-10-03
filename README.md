# Predicting Employee Attrition Using HR Analytics

This project focuses on predicting employee attrition using the IBM HR Analytics Employee Attrition dataset. By analyzing various factors like satisfaction levels, compensation, job involvement, and workload, this analysis aims to identify employees who are at risk of leaving the company. The project also explores key drivers of turnover and presents actionable insights for improving employee retention.

## Project Objective

To develop a model that predicts which employees are at risk of leaving and to identify the major factors contributing to employee attrition.

## Data Sources

- **Employee Attrition Data**: [IBM HR Analytics Employee Attrition & Performance dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

## Methods and Tools

- **Data Cleaning and Preprocessing**: Python, Pandas
- **Exploratory Data Analysis (EDA)**: Visualizations using Matplotlib and Seaborn
- **Machine Learning Models**: XGBoost classifiers using scikit-learn and XGBoost to predict attrition and identify at-risk employees
- **Dashboard**: Created an interactive dashboard using Power BI to visualize key metrics and predictions for HR departments

## Key Findings

- **Satisfaction and Overtime are Major Drivers**: Low job satisfaction, poor work-life balance, and regular overtime are strong indicators of attrition.
- **Younger Employees and Shorter Tenure at Risk**: Younger employees and those with less time in their current role or with their current manager are more likely to leave.
- **Low Compensation Increases Attrition Risk**: Employees in the lowest income brackets show the highest attrition rates, emphasizing the importance of competitive pay.
- **Model Performance**: The Random Forest and XGBoost models were able to identify at-risk employees, with a balanced accuracy of 87%. Precision and recall for identifying those who left were lower (52%) due to the inherent class imbalance in the data.

## Full Analysis

The full can be found at my [website]().

## Repository Contents

- **data/**: Contains the dataset used in the project
- **images/**: Contains images of the dashboard and key visualizations used in the analysis
- **dashboard/**: Power BI dashboard file for visualizing employee attrition metrics and predictions
- **notebooks/**: Jupyter notebooks with data preprocessing, model development, and analysis code

## Future Research Directions

- **Expand Dataset**: Use time-based data to track employee behavior over time for a more dynamic model.
- **Explore Additional Factors**: Incorporate qualitative data like employee feedback or survey results to improve the predictive power of the model.
- **Model Refinement**: Investigate advanced techniques for handling class imbalance to improve recall for employees likely to leave.
- **Intervention Strategies**: Develop predictive models that suggest tailored interventions based on identified risk factors.

## Acknowledgements

- IBM and kaggle user pavansubhasht, for providing the HR Analytics dataset used in this project
