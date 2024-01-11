# Customer-Churn-Analysis
![Customer-Churn](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/6ce66136-9662-4145-b71c-a9ed122b9cd7)


## Project Overview
Customer churn, the phenomenon where customers discontinue using a product or service. Identifying and mitigating customer churn is crucial for sustaining business growth and profitability. This project aims to leverage advanced analytics and machine learning techniques to predict customer churn in a telecom industry, enabling proactive retention strategies for the organization.
## Table Of Contents
- [Introduction](#Intoduction)
- [Data Description](# Data Description)
- [Methodology](#Methodology)
    - [Data Cleaning]( #DataCleaning)
    - [EDA](#ExploratoryDataAnalysis)
    - [Model Building](#ModelBuilding )
 - [Conclusion and Key Insights](#ConclusionsAndKeyInsights) 


## Intoduction
In this case study, end to end Exploratory Data Analysis has been performed, and idenfitied the characteristics of the customers that are more likely to churn, followed by an implementation of various machine learning tools and techniques to predict customer churn for a telecom company.

## Data Description
The Dataset summarizes the usage behavior of about 7000 active users of this telecom service. The file is at a customer level with 19 variables.
Data can be accessed from[ here](https://github.com/deepanshak/Customer-Churn-Analysis/blob/main/WA_Fn-UseC_-Telco-Customer-Churn.csv)
## Methodology
### Data Cleaning
- Checking for null and duplicate values.
- Removing missing values.
- changing data types for some variables.
- claculating max tenure and grouping it to bins of 12 months.
- dropping unnecessary variables.
### Exploratory Data Analysis 
Univariate Analysis
- churn count based on various variables like gender, senior citizen, dependents,tenure_group.
  
- Relation between monthly charge and total charges.
  
![rs bw monthly charge and total charge](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/5c225da6-3452-4b14-84d7-ddb896c3a18d)

- Monthly charges and total charges by churn.
  
  ![total charges by churn](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/835f7231-3d5f-456c-886f-6097fb9967fa)

  
![monthly charges by churn](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/0dd1668b-6dd2-4ecd-9dc8-f4426f15722f)

- Building a correlation of all predictors with Churn.
  ![correlation with all predictors](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/f55e696d-205c-46de-90a8-a52f53d12400)


- Heat map plot to show relation between variables.
 
 ![heat map](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/c34e2d4d-0a8d-4fa8-803f-e65055d9ac96)

Bivariate Analysis
- Gender for churned and non churned customers.
- Distribution of payment for churned & non churned customers.
- Distribution of senior citizen for churned & non churned customers.
  ![distribution of senior citizen for churned customer](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/b75f2b54-52dd-43ef-aa56-4798dbf1508b)

- Tech support for churned & non churned customers
- Distribution of contract for churned & non churned customers.
  ![contract distribution for churned customer](https://github.com/deepanshak/Customer-Churn-Analysis/assets/139687677/48c36db1-b307-4f28-a270-038b4da488fe)

For complete analysis refer to file:[EDA](https://github.com/deepanshak/Customer-Churn-Analysis/blob/main/Churn%20Analysis%20-%20EDA.ipynb)
### Model Building 
Refer to file for [model building](https://github.com/deepanshak/Customer-Churn-Analysis/blob/main/Churn%20Analysis%20-%20Model%20Building.ipynb)
#### Data Prepration
- Defining the input variable and target variable.
- Splitting the data into training and test sets.
#### Algorithms Used:
- [Decision Tree Classifire](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
- [Random Forest Classifire](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [principal Component analysis](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
- [SMOTE ](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)
#### Model Evaluvation
The algorithm showing the most optimum result is choosen based on various metrices like R^2 score, classification Report of predicted and Test variables and using confusion matrix.
#### Pickled Model 
Pickled the Random Forest model to import the model without loading this entire ipynb file, and utilize it for predictions.
## Conclusions And Key Insights

These are some of the quick insights from this case study:

1. Electronic check medium are the highest churners
2. Contract Type - Monthly customers are more likely to churn because of no contract terms, as they are free to go customers.
3. No Online security, No Tech Support category are high churners
4. Non senior Citizens are high churners

