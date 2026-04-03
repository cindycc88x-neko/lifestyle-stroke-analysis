# Lifestyle Factors and Stroke Risk Analysis

## Project Overview
This project explores the relationship between lifestyle factors and stroke risk using a healthcare dataset. The goal is to identify potential risk indicators and evaluate whether lifestyle-related variables can be used to predict stroke occurrence.

## Dataset
The dataset includes demographic and health-related information such as age, BMI, glucose level, smoking status, and work type.

## Methods

### 1. Exploratory Data Analysis
We examined the relationship between several lifestyle factors and stroke risk:

- Smoking status
- Work type
- Marital status
- Body Mass Index (BMI)
- Average glucose level

Bar charts were used to compare stroke rates across different categories.

### 2. Key Findings

- Individuals with higher glucose levels showed a significantly higher stroke rate.
- Smoking history appears to be associated with increased stroke risk.
- Work type and marital status may reflect underlying demographic and lifestyle differences.
- BMI showed a weaker but noticeable association.

### 3. Data Preprocessing

- Missing BMI values were filled using the mean.
- Categorical variables were transformed using one-hot encoding.

### 4. Model

A Logistic Regression model was used to predict stroke risk.

- Class imbalance was handled using `class_weight='balanced'`.
- Features included:
  - BMI
  - Glucose level
  - Smoking status
  - Work type
  - Marital status

### 5. Results

- Accuracy: 0.67
- Recall (stroke cases): 0.61
- Precision (stroke cases): 0.10

The model demonstrated a moderate ability to identify stroke cases, though with a high false positive rate.

## Discussion

The results suggest that lifestyle factors, particularly glucose level and smoking, are associated with stroke risk.

In a healthcare context, prioritizing recall is often more important than precision, as identifying high-risk individuals is critical for early intervention.

## Conclusion

This project highlights the potential of using lifestyle-related variables to assess stroke risk. Further improvements could include additional clinical variables and more advanced models.
