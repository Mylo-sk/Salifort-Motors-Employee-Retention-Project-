# Salifort Motors Employee Retention Project

## 1. Background and Overview

Salifort Motors, an alternative energy vehicle manufacturer, is experiencing high employee turnover. The senior leadership team seeks to understand the causes of attrition and identify employees at risk of leaving. This project analyzes HR data to uncover key factors driving turnover and builds a predictive model using logistic regression to assist with proactive retention strategies.

## 2. Data Structure Overview

The dataset contains 15,000 records of employee information across the following fields:

| Variable | Description |
|----------|-------------|
| satisfaction_level | Employee-reported job satisfaction (0–1) |
| last_evaluation | Score of last performance review (0–1) |
| number_project | Number of active projects |
| average_monthly_hours | Average monthly hours worked |
| time_spend_company | Tenure in years |
| Work_accident | Work accident (Yes/No) |
| promotion_last_5years | Promoted in last 5 years (Yes/No) |
| Department | Employee department |
| salary | Salary level (low, medium, high) |
| left | Employee left (1 = Yes, 0 = No) |

> **Note**: All categorical variables were encoded for modeling, and numerical features were scaled using `StandardScaler`.

## 3. Executive Summary

- **Satisfaction level** is the strongest predictor of attrition. Low satisfaction correlates directly with turnover.
- Employees working **excessive hours** or on **many projects** show increased attrition.
- **No recent promotions** and **longer tenure (≥ 4 years)** increase the likelihood of leaving.
- The logistic regression model achieved an **accuracy of 77%** with good balance between **precision** and **recall**.

| Metric        | Score |
|---------------|-------|
| Accuracy      | 0.77  |
| Precision     | 0.71  |
| Recall        | 0.58  |
| F1 Score      | 0.64  |

## 4. Insights Deep Dive

### 1. **Satisfaction Level**
- Employees with satisfaction < 0.5 had the highest turnover rate (over 60% left).
- Improving job satisfaction could significantly reduce attrition.

### 2. **Project Load**
- Employees engaged in **more than 5 projects** were much more likely to leave.
- This suggests overwork may be contributing to dissatisfaction and attrition.

### 3. **Tenure and Promotion**
- Employees with **4–6 years** at the company and **no promotions** in the past 5 years left at higher rates.
- Promotion stagnation appears to be a turnover driver.

### 4. **Work Accidents**
- Surprisingly, employees with no recorded accidents had higher attrition, possibly due to less engagement or different role types.

## 5. Recommendations

- **Monitor and boost satisfaction levels**, particularly among overworked employees.
- **Reassess project distribution** to prevent burnout.
- **Introduce career development programs** and regular performance reviews for mid-tenure employees.
- **Develop early warning systems** using the logistic regression model to flag at-risk staff.

These actions can improve job satisfaction and reduce turnover-related costs.

## 6. Caveats and Assumptions

- The dataset does not include qualitative data like exit interviews or manager feedback.
- Salary data is limited to three tiers and may not reflect full compensation dynamics.
- The dataset is static; trends may shift over time.

---

### 🔗 Technical Details

View the full notebook and code:
👉 [Salifort_Motors_Employee_Retention_Project.ipynb]((https://github.com/Mylo-sk/Salifort-Motors-Employee-Retention-Project-/blob/main/Salifort_Motors_Project.ipynb))

---



