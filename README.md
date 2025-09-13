# Telecommunications Analysis

## Authors
Neema Naledi,
Elsie Almadi,
Elvis Wanjohi,
Stephen Gachingu,
Mark Muriithi.

## 1.Business Understanding
*__1.1 Overview__*

SyriaTel is a telecommunication company that specializes in the provision of data and voice services. Like its competitors, the company’s overarching goal is profit maximization. However, one of the major challenges it faces is customer churn, which occurs when subscribers cancel their services and switch to competitors. This project seeks to address that challenge through data-driven methods

*__1.2 The Problem__:* 

 SyriaTel is losing a significant amount of revenue because many customers are canceling their services. At present, the company does not have a reliable system to predict which customers are most likely to leave. Without such a system, it is difficult to intervene in time to retain customers, which ultimately leads to reduced profits and loss of market share.
 
*__1.3 Objectives__:* 

The main business objective is to reduce customer churn by predicting which customers are at risk of leaving. Achieving this will allow SyriaTel to take timely action and improve customer retention

*__1.4 Project Objectives__*

Main Objective
The main objective of this project is to develop a machine learning classifier that can accurately predict whether a SyriaTel customer is likely to churn.

Specific Objectives
The specific objectives of the project are:

1. To analyze customer attributes and usage patterns in order to identify the key drivers of churn.
2. To develop, train, and evaluate predictive models that classify customers as churners or non-churners.
3. To generate actionable business insights and recommendations, based on the model outputs, that can support strategies to reduce customer churn.

*__1.5 Research Questions__*

The project is guided by the following research questions:

1. What characteristics are most strongly associated with customers who churn?
2. Which machine learning algorithm provides the best predictive performance for churn classification?
3. How can the insights from the churn model be applied to design effective customer retention strategies?

*__1.6 Success Criteria__:* 

The success of this project will be assessed in three ways. First, it should generate actionable insights that SyriaTel can use to reduce churn rates in the future. Second, the predictive model should achieve acceptable levels of performance, with high accuracy and a strong ability to correctly identify customers who are likely to leave. Finally, the results should be presented in a way that is clear and interpretable, so that they can be easily understood and applied by business managers and decision-makers

## 2. Data Understanding
**Data set used**:

 Our analysis stems from the {https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset} from kaggle.
It contains customer account and usage information for a telecommunications company.

The dataset does not specify the time frame; it is a cross-sectional snapshot of customer behavior.

It consists of 3,333 rows and 21 columns.

The target variable is churn. This is a binary variable that indicates whether a customer has churned (True) or not (False). Since the target is categorical, it will be encoded during data preparation to allow machine learning models to process it.


**Outliers**: 
Why we decided to keep outliers:

1. customer behavior naturally varies widely.
2. Heavy users who suddenly reduce usage might be prime churn candidates. These patterns are crucial for retention strategies
3. Customers with extremely high usage are often the most profitable clients and removing them would eliminate key revenue insights


## 3. Data Preparation

In this section the Syria Tel dataset is prepared for analysis by cleaning, transforming and standardizing the data. The goal is to ensure accuracy, handle missing values, and make the dataset ready for further exploration and modeling.

We started by getting the necessary libraries to analyse our data. We imported pandas for data manipulation, Numpy for numerical operations, seaborn and matplotlib for visualizations of patterns and trends

We loaded our data into a dataframe called Syriatel_data then proceeded to look at our dataset which contained 3333 rows and 21 columns. 

We then looked for which of our columns are numerical and which are categorical 


1. __*Data Cleaning*__

Upon inspection of the dataset, we found it had no missing values or duplicated items. 

2. __*Data Manipulation*__

We then added columns that we deemed useful in our analysis. We changed our area code column to an object rather than it being an integer as it is categorical. The phone number column was dropped as it was not necessary for our analysis. We followed by standardizing our columns so that our model can be effective.

3. __*Exploratory Data Analysis*__

Next we generated visualisations to check for the relationship between the features especially  '#churn' as it is our target variable.  WE used bar graphs, correlation plots, distribution plots and kde plot for our visuals.

## 4. Modeling
We resampled the data to address the issue of class imbalance by using SMOTE and Stratified sampling so that the models can learn from both classes

We used the train test split split method to split the data into training and testing sets using a ```70/30 split

2 models were used to model our data i.e logistic regresion and decision trees to find out which trained our data better.




## 5. Evaluation
Precision, recall and f1 score were used to evaluate our modells and plotted a bar graph to show the results..

ROC curves were plotted and AUC scores calculated so as to do a comparison of the curves of the 2 models

We plotted a confusion matrix to see where our True and False Positives and Negatives lie 

## 6. Key Findings
__1. Logistic Regression__:

* AUC = 0.808
* This means Logistic Regression is good at separating churn vs. non-churn customers, with about 81% ability to rank positive cases higher than negative cases.
* The curve is well above the diagonal baseline (random guessing), showing strong predictive power.

__2. Decision Tree (blue curve):__

* AUC = 0.793
* Very close to Logistic Regression in performance, but slightly lower.
Still much better than random guessing.

__3. Comparison:__

* Both models perform almost equally well in terms of AUC.
* Logistic Regression has a small edge in separating churners from non-churners

## Insights
* Both models agree:
customer service calls are a strong churn indicator where it affects churn both positively or negatively depending on how a customer is treated .
* Different perspectives:
Logistic highlights plans and customer service interaction.
Decision Tree highlights usage and billing behavior.
* Business impact:
Improve customer support quality to reduce churn.
Revisit international plan pricing.
Offer loyalty rewards for heavy users to reduce churn risk.
## 7. Reccomendations 
__1. Improve Customer Support Quality__

* High service call volume is strongly tied to churn.
* Invest in better training, quicker resolutions, and proactive issue handling.

__2. Reassess International Plan Pricing & Policies__

* International plan customers churn more.
* Review pricing, offer bundled discounts, or add loyalty incentives to retain them.

__3. Retain High-Usage Customers__

Heavy day-minute users are at lower risk of churning but we've to keep the customers satisfied by creating targeted retention programs (loyalty points, discounted packages, or “VIP customer” care) to reduce churn on loyal customers.


## Technologies Used
- Python: Primary programming language
- Pandas: Data manipulation and analysis
- Matplotlib: Data visualization
- Jupyter Notebook: Development environment
- Git: Commit and push to remote repository


## Support
For questions or support, please contact:
naledineema@gmail.com, leeelvis562@gmail.com, aginalmadi@gmail.com, mark.muriithi@gmail.com and 


