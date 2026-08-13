# Factors Influencing Customers' Online Purchasing Decisions
## Project Overview

This is an academic project about understanding customers' online shopping behavior and the factors related to their purchase decisions. The project uses the **Online Shoppers Intention** dataset from Kaggle, which contains information about how users interact with an e-commerce website, such as the number of product pages they visit, the time they spend on product pages, bounce rate, exit rate, and page value.

---

## Business Problem

In e-commerce, attracting website visitors does not necessarily lead to purchases. Understanding how customers interact with a website can help businesses identify behaviors associated with higher purchase intent.
The main question of this project is: **"Which customer browsing and website interaction features are most important for predicting an online purchase decision?"**

---

## Project Objectives

- Explore customers' browsing and interaction behavior.
- Identify important features associated with online purchase decisions.
- Select the most useful features for the prediction model.
- Build a machine learning model to predict customers' online purchase decisions.
- Evaluate the predictive performance of the model.
- Turn the results into practical business insights.

---
## Dataset

**Dataset:** Online Shoppers Intention  
**Source:** Kaggle  
**Target Variable:** `Revenue`  
The `Revenue` variable represents whether the user's website session resulted in a purchase:

True --> Purchase  
False --> No purchase  

The dataset contains behavioral information about users during their website sessions, including the number of product-related pages viewed, time spent on product-related pages, bounce rate, exit rate, page value, and other session characteristics.

---

## Analysis & Methodology
The project follows these main steps:

1. Data Preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature Selection
4. Gradient Boosting Classification
5. Model Evaluation
6. Business Insights

---

## Feature Selection

SelectKBest with Mutual Information was used to identify the most relevant features.

The five selected features were:

- `ProductRelated`
- `ProductRelated_Duration`
- `BounceRates`
- `ExitRates`
- `PageValues`

---

## Machine Learning

A **Gradient Boosting Classifier** was developed to predict whether a customer would make an online purchase.

---

## Key Results

The Gradient Boosting Classifier achieved:  
**Accuracy: 88.3%**  
The model performed particularly well in identifying customers who did not make a purchase.
For the purchase class, the model achieved:

- Precision: 0.63
- Recall: 0.74 
- F1-score: 0.68

`PageValues` was identified as the most important feature in the model.

---

## Business Insights

The analysis indicates that:

- Customers who view more product-related pages tend to show stronger purchase behavior.
- Spending more time on product-related pages is associated with higher purchase intent.
- Higher BounceRates and ExitRates are associated with users who do not complete a purchase.
- `PageValues` has the strongest contribution to the prediction model.

