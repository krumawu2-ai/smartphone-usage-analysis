# smartphone-usage-analysis
Exploratory data analysis of smartphone usage behavior
# Smartphone Usage & Work Productivity Analysis

## Overview

This project investigates whether smartphone usage behaviors are related to work productivity. Using a dataset containing behavioral metrics such as phone usage hours, social media usage, sleep patterns, stress levels, and caffeine intake, I conducted a complete data science workflow including data preprocessing, exploratory data analysis (EDA), feature engineering, and predictive modeling.

The goal of this project was to determine whether smartphone usage patterns could meaningfully predict **work productivity scores**.

---

## Dataset

The dataset contains behavioral data from approximately **50,000 users** and includes the following variables:

| Feature | Description |
|--------|-------------|
| User_ID | Unique identifier for each user |
| Age | Age of the user |
| Gender | Gender category |
| Occupation | User's occupation |
| Device_Type | Smartphone device type |
| Daily_Phone_Hours | Average daily smartphone usage |
| Social_Media_Hours | Daily time spent on social media |
| Work_Productivity_Score | Productivity score (target variable) |
| Sleep_Hours | Average sleep duration |
| Stress_Level | Self-reported stress level |
| App_Usage_Count | Number of apps used per day |
| Caffeine_Intake_Cups | Daily caffeine intake |
| Weekend_Screen_Time_Hours | Weekend phone usage |

Additional engineered features were created during the analysis process.

---

## Project Workflow

### 1. Data Preprocessing

- Loaded the dataset using **Pandas**
- Investigated missing values
- Verified variable types
- Handled encoding issues when loading the dataset
- Converted appropriate variables to categorical types

---

### 2. Exploratory Data Analysis (EDA)

Several visualizations were used to explore patterns and relationships between variables:

- Correlation heatmaps
- Scatter plots
- Box plots
- Distribution plots

These visualizations helped identify relationships between smartphone usage behaviors and productivity.

---

### 3. Feature Engineering

Additional features were created to better capture behavioral patterns:

- **Social_Media_Ratio**
- **Sleep_Deficit**
- **Weekend_Extra_Usage**

These engineered variables provided additional behavioral context in the analysis.

---

### 4. Feature Selection

Behavioral variables used for modeling included:

- Daily_Phone_Hours
- Social_Media_Hours
- Sleep_Hours
- Stress_Level
- Caffeine_Intake_Cups
- Weekend_Screen_Time_Hours
- App_Usage_Count

---

### 5. Modeling

A **Linear Regression model** was built as a baseline predictive model to evaluate whether smartphone usage behavior could predict productivity.

Model evaluation metrics included:

- **R² (Coefficient of Determination)**
- **RMSE (Root Mean Squared Error)**

---

## Key Findings

### Weak Relationships with Productivity

Correlation analysis revealed that most variables had **near-zero correlation with Work_Productivity_Score**.

This suggests that smartphone usage behaviors in the dataset do not meaningfully explain productivity variation.

---

### Model Performance

The linear regression model produced:

R² ≈ 0  
RMSE ≈ 2.9

An R² value near zero indicates that the model performs no better than predicting the average productivity score.

---

### Interpretation

The results suggest that smartphone usage alone is **not a strong predictor of productivity** in this dataset. Productivity likely depends on additional factors not captured in the dataset, such as:

- work environment
- job complexity
- motivation
- psychological factors
- task structure

---

## Visualizations

Key visualizations generated during the analysis include:

- Correlation heatmap of behavioral variables
- Scatter plot of **Daily Phone Usage vs Productivity**
- Stress level distributions across occupations

These visualizations helped confirm the lack of strong relationships between smartphone usage and productivity.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Structure

```
smartphone-productivity-analysis
│
├── data
│   └── Smartphone_Usage.csv
│
├── notebooks
│   └── smartphone_analysis.ipynb
│
├── visuals
│   ├── correlation_heatmap.png
│   ├── productivity_scatter.png
│   └── stress_boxplot.png
│
├── requirements.txt
└── README.md
```

---

## Conclusion

This project demonstrates a complete **data science workflow**, including data preprocessing, exploratory analysis, feature engineering, and predictive modeling.

Although the dataset did not produce strong predictive relationships, the analysis highlights the importance of **exploratory data analysis and honest model evaluation** when interpreting the limits of available data.

---

## Author

Kudakwashe Rumawu  
Data Science | Analytics | Machine Learning
