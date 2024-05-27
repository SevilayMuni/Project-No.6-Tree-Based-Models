
# Random Forest Assisted Suggestions for Salifort Motors Employee Retention

Salifort Motors wants to improve employee retention and learn what determines whether employee leave or stay in the company.
I built logistic regression and tree-based machine learning models. The final random forest model performed with:
- precision of 97.7%
- recall of 92.5%
- accuracy of 98.4%

All in all, I created powerful both decision tree and random forest models and uncovered important variables for employee retention: 
- satisfaction level of employee
- performance review of employee
- number of projects employee contributes
- tenure
- overwork

## Business Understanding
The HR department at Salifort Motors wants to improve employee satisfaction levels and answer following question: what’s likely to make the employee leave the company?

The project goals: 
- analyzing the data collected by the HR department
- build a model that predicts whether or not an employee will leave the company
- identify factors that contribute to their leaving 

#### Since finding, interviewing, and hiring new employees are time-consuming and expensive, increasing employee retention will be beneficial to the company.
## Modeling and Evaluation
#### Identifying the prediction type and model
Modeling purpose is predicting whether an employee leaves the company (categorical outcome variable). The outcome variable can be either 1 (employee left) or 0 (employee stayed).
- It is binary classification task

Since the outcome variable is categorical and task is binary classification, appropriate models:
- Logistic Regression 
- Tree-based Machine Learning models

#### Model Evaluation Metrics
- AUC: area under the ROC curve; it's also considered the probability that the model ranks a random positive example more highly than a random negative example.
- Precision: measures the proportion of data points predicted as True that are actually True.
- Recall: measures the proportion of data points that are predicted as True, out of all the data points that are actually True. In other words, it measures the proportion of positives that are correctly classified.
- Accuracy: measures the proportion of data points that are correctly classified.
- F1-score: aggregation of precision and recall.

## Model Results
    Decision Tree    Precision  Recall  F1    Accuracy  AUC
                     0.977      0.915   0.945  0.982     0.967

    Random Forest    Precision  Recall  F1    Accuracy  AUC
                     0.983      0.913   0.947 0.983     0.980

    2nd Decision Tree Precision Recall  F1    Accuracy  AUC
                      0.959     0.909   0.933 0.978     0.959


    2nd Random Forest Precision Recall  F1    Accuracy  AUC
                      0.976     0.908   0.941 0.981     0.977
## Data Understanding

- Employees in the company are overworked.
- Everyone with seven projects left the company, and avg. working hours of this group and those who left with six projects were noticeably higher than any other group.

- Mean working hours increases with number of projects worked.
- There are two groups of employees who left the company: 1) those who worked considerably less than their collegues with the same number of projects 2) those who worked much more. For 1) it’s possible that they were fired. Also, this group might include employees who had already given their notice and were assigned fewer hours. For 2) they probably quit. 

- The optimal number of projects for employees to work on is 3; the ratio of left/stayed is very small for this group.

- Very few employees were promoted in the last 5 years. In spite of working very long hours, few of those employees were promoted.
- All of the employees who left the company were working the longest hours.

- The mean and median satisfaction scores of employees who left are lower than those of employees who stayed.

- Employees who left can be grouped under 2 categories: 1) Dissatisfied employees w/ shorter tenures 2) Very satisfied employees w/ medium-length tenures.
- Four-year employees who left have an unusually low satisfaction level. 
- The longest-tenured employees didn’t leave. 
- If an employee has spent more than six years at the company, they stay.
- 7 and 8 year tenured employees with low salary had high satisfaction level (more than their high salary earning peers). 
*This implies that long-tenured employee satisfaction might be weakly correlated to salary.*


- **Leaving** is linked to **longer working hours, contributing to many projects, and lower satisfaction levels.**
- *Working long hours and not receive promotions or good evaluation scores might chasing employees away*
- Employees are leaving the company as a result of poor management. 
## Insights
➢ Cap the number of projects that employees contributes

➢ Consider promoting employees who have been working for at least 4 years

➢ Conduct further analysis on why four-year tenured employees are so dissatisfied

➢ Either provide compensation to employees for working longer hours, or don’t require
them to do so

➢ If employees aren’t familiar with the company’s overtime pay policies, inform them
about

➢ High evaluation scores should not be restricted to employees who work 200+ h/month

➢ Improve performance review process
## Acknowledgements
Data Source:
https://www.kaggle.com/giripujar/hr-analytics

CC0: Public Domain

readme.so



## Variables

Variable  |Description |
-----|-----|
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]|
last_evaluation|Score of employee's last performance review [0&ndash;1]|
number_project|Number of projects employee contributes to|
average_monthly_hours|Average number of hours employee worked per month|
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)# Project-No.6-XGBoost-RandomForest
# Project-No.6-XGBoost-RandomForest
# Project-No.6-XGBoost-RandomForest
