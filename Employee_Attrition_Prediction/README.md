# Employee Attrition Prediction | Supervised Machine Learning

## 1. Project Overview

This project predicts whether an employee is likely to leave a company.
It uses supervised machine learning and Logistic Regression for binary classification.
A baseline model is compared with L1 and L2 regularized models.

## 2. Problem Statement

A company is experiencing an increase in employee resignations.
Turnover can increase recruitment costs, delay projects, and result in loss of skilled talent.
The HR department needs a model to predict employee turnover from work-related factors.

## 3. Objectives

- Build a baseline Logistic Regression model.
- Apply L1 (Lasso) and L2 (Ridge) regularization.
- Compare model performance and recommend the best-performing model.

## 4. Dataset

- File: `EmployeeAttritionPrediction.csv`
- Records: 900 | Columns: 15
- Target: `Employee_Turnover` (`1` = Left, `0` = Stayed)

### Features

| Feature                                   | Description                          |
| ----------------------------------------- | ------------------------------------ |
| `Job_Satisfaction`                        | Job satisfaction level               |
| `Performance_Rating`                      | Employee performance score           |
| `Years_At_Company`                        | Years worked at the company          |
| `Work_Life_Balance`                       | Work-life balance                    |
| `Distance_From_Home`                      | Distance from workplace              |
| `Monthly_Income`                          | Monthly salary                       |
| `Education_Level`                         | Education qualification level        |
| `Age`                                     | Employee age                         |
| `Num_Companies_Worked`                    | Previous companies worked at         |
| `Employee_Role`                           | Encoded job role                     |
| `Annual_Bonus`                            | Annual bonus received                |
| `Training_Hours`                          | Training hours attended              |
| `Department`                              | Encoded department                   |
| `Annual_Bonus_Squared`                    | Engineered feature: bonus squared    |
| `Annual_Bonus_Training_Hours_Interaction` | Bonus and training-hours interaction |

## 5. Tools and Libraries

- Python
- Jupyter Notebook
- Pandas
- Scikit-learn

## 7. Machine Learning Workflow

1. Load the dataset using Pandas.
2. Separate features (`X`) and target (`y`).
3. Split the data into training and testing sets.
4. Train baseline, L1, and L2 models; generate test-set predictions.

## 8. Train-Test Split

The notebook uses `train_test_split` with:

- Training set: 80%
- Testing set: 20%
- `random_state=42`

## 9. Models Implemented

### Baseline Logistic Regression

- Standard Logistic Regression model.

### L1 Regularization (Lasso)

- Applies L1 penalty, which can reduce some coefficients to zero.

### L2 Regularization (Ridge)

- Applies L2 penalty, shrinking coefficients towards zero.

## 10. Evaluation Metrics

The notebook uses `accuracy_score` and `classification_report`.

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Correct positive predictions among all positive predictions.
- **Recall:** Correctly identified positive cases among all actual positive cases.
- **F1-score:** Harmonic mean of precision and recall.
- **Support:** Number of actual samples in each class.

## 11. Model Results

| Model                              | Test Accuracy |
| ---------------------------------- | ------------: |
| Baseline Logistic Regression       |        85.93% |
| L1 Regularized Logistic Regression |        87.04% |
| L2 Regularized Logistic Regression |        85.93% |

### Result Analysis

- L1 regularization achieved the highest test accuracy.
- Baseline and L2 achieved the same test accuracy.
- Class `1` F1-score: Baseline `0.84`, L1 `0.86`, Ridge `0.84`.

## 12. Conclusion

L1 regularized Logistic Regression performed best among the three tested models.
It achieved a test accuracy of approximately 87.04%.
It is the recommended model based on the current notebook evaluation.
This conclusion is limited to the models, parameters, and test split used.

## 15. Author

**Manasvi Patidar**
