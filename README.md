# Lifestyle Factors and Stroke Risk Analysis

## Background

Stroke is one of the leading causes of death and disability worldwide. While clinical factors such as hypertension and heart disease are well studied, lifestyle factors may also play an important role in stroke risk.

Understanding how lifestyle-related variables influence stroke risk can support early prevention and public health strategies.

---

## Objective

This project aims to investigate the relationship between lifestyle factors and stroke risk, and evaluate whether these variables can be used for predictive modelling.

---

## Dataset

* Source: Kaggle Stroke Dataset
* Features include:

  * Smoking status
  * BMI
  * Average glucose level
  * Work type
  * Marital status
  * Stroke outcome (target variable)

---

## Exploratory Data Analysis

### Stroke Rate by Smoking Status

![Smoking Analysis](https://github.com/cindycc88x-neko/lifestyle-stroke-analysis/blob/main/smoking.jpg?raw=true)

Individuals with a history of smoking show a higher stroke rate, suggesting lifestyle-related risk.

---

### Stroke Rate by Marital Status

![Marital Analysis](https://github.com/cindycc88x-neko/lifestyle-stroke-analysis/blob/main/marital.jpg?raw=true)

Marital status appears associated with stroke risk, possibly reflecting age and social factors.

---

### Stroke Rate by Work Type

![Work Type Analysis](https://github.com/cindycc88x-neko/lifestyle-stroke-analysis/blob/main/work.jpg?raw=true)

Different work categories show variation in stroke rates, indicating potential socioeconomic influences.

---

### BMI and Glucose Level by Stroke Status

![BMI and Glucose](https://github.com/cindycc88x-neko/lifestyle-stroke-analysis/blob/main/bmi%20&%20glucose.jpg?raw=true)

Stroke patients tend to have higher average glucose levels, while BMI shows a smaller difference.

---

## Data Preprocessing

* Missing BMI values were filled using the mean
* Categorical variables were converted using one-hot encoding

---

## Modeling

### Model Used

* Logistic Regression

### Handling Class Imbalance

To address the imbalance in stroke cases:

```python
class_weight='balanced'
```

---

## Model Performance

| Metric             | Value |
| ------------------ | ----- |
| Accuracy           | ~0.67 |
| Recall (Stroke)    | ~0.61 |
| Precision (Stroke) | ~0.10 |

---

## Key Insights

* Glucose level is strongly associated with stroke risk
* Smoking and lifestyle factors show potential influence
* Model prioritises recall, aligning with healthcare risk detection
* Class imbalance significantly affects performance

---

## Conclusion

This project highlights the importance of lifestyle factors in stroke risk assessment. While predictive performance is limited, the model demonstrates potential for identifying high-risk individuals.

---

## Tools Used

* Python
* Pandas
* Matplotlib
* Scikit-learn

---

## Author

Shuran Cui
MSc Health Data Science (Incoming), University of Manchester
