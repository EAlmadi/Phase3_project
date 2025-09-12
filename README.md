# Telecommunications Analysis

## Authors
Neema Naledi,
Elsie Almadi,
Elvis Wanjohi,
Stephen Gachingu,
Mark Muriithi.

## 1.Business Understanding
 * __1.1 Overview__*

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

To analyze customer attributes and usage patterns in order to identify the key drivers of churn.
To develop, train, and evaluate predictive models that classify customers as churners or non-churners.
To generate actionable business insights and recommendations, based on the model outputs, that can support strategies to reduce customer churn.

*__1.5 Research Questions__*

The project is guided by the following research questions:

What characteristics are most strongly associated with customers who churn?
Which machine learning algorithm provides the best predictive performance for churn classification?
How can the insights from the churn model be applied to design effective customer retention strategies?

*__1.6 Success Criteria__:* 

The success of this project will be assessed in three ways. First, it should generate actionable insights that SyriaTel can use to reduce churn rates in the future. Second, the predictive model should achieve acceptable levels of performance, with high accuracy and a strong ability to correctly identify customers who are likely to leave. Finally, the results should be presented in a way that is clear and interpretable, so that they can be easily understood and applied by business managers and decision-makers

## 2. Data Understanding
**Data set used**:

 Our analysis stems from the [https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset] from kaggle.
It contains customer account and usage information for a telecommunications company.

The dataset does not specify the time frame; it is a cross-sectional snapshot of customer behavior.

It consists of 3,333 rows and 21 columns.

The target variable is churn. This is a binary variable that indicates whether a customer has churned (True) or not (False). Since the target is categorical, it will be encoded during data preparation to allow machine learning models to process it.

**Reasons for data selection**:


**Outliers**: 
Why we decided to keep outliers:

1. customer behavior naturally varies widely.
2. Heavy users who suddenly reduce usage might be prime churn candidates. These patterns are crucial for retention strategies
3. Customers with extremely high usage are often the most profitable clients and removing them would eliminate key revenue insights

**Merged Data**:


## Data Preparation
1. __*Data Cleaning*__


2. __*Added Calculated Columns*__


## Modeling
__Visual Data Analysis:__


## Evaluation


## Prerequisites
*Getting started*
1. Fork 
Create a fork.

2. Clone 

- Type: git clone
(you can clone using either *SSH key*  or the *HTTPS*)
[(https://github.com/EAlmadi/Phase3_project.git)]

## Key Findings


## Reccomendations 
1. 
2. 
3. 

## Testing
To run the cells press ctrl+shift
You'll need to download the dataset required 
You can get the dataset from:
[https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset]

## Technologies Used
- Python: Primary programming language
- Pandas: Data manipulation and analysis
- Matplotlib: Data visualization
- Jupyter Notebook: Development environment
- Git: Commit and push to remote repository

## Contributions
Contributions to the Telecommunications Analysis are welcome! If you have any suggestions, bug fixes, or additional features you'd like to add to the dashoard, please feel free to submit a pull request or open an issue.

## Support
For questions or support, please contact:
naledineema@gmail.com,


