# Analysis Report

## Data Preprocessing

Before starting the analysis, the Online Shoppers Intention dataset was checked and prepared for the machine learning process.

The main preprocessing steps included:

- Checked for missing values. None were found.
- Converted `Weekend` and `Revenue` from Boolean (`True/False`) to binary (`1/0`).
- Used One-Hot Encoding for `Month` and `VisitorType`.
- Used `StandardScaler` to standardize selected numerical features, including `Administrative_Duration`, `Informational_Duration`, `ProductRelated_Duration`, `BounceRates`, `ExitRates`, and `PageValues`.

---

## Exploratory Data Analysis

EDA was used to explore customer behavior on the website. The analysis compared sessions where customers made a purchase with sessions where they did not.

The main variables looked at were product page views, time spent on product pages, bounce rate, exit rate, and page value.

---

## Feature Selection

SelectKBest with Mutual Information was used to select the features most related to the target variable `Revenue`.

The five selected features were:

- `ProductRelated`
- `ProductRelated_Duration`
- `BounceRates`
- `ExitRates`
- `PageValues`

These five features were then used to train the Gradient Boosting Classifier.

---

## Machine Learning Model

A **Gradient Boosting Classifier** was used to predict whether a customer would make an online purchase.

The model was trained using the selected features and evaluated on the test dataset.

---

## Model Evaluation

The Gradient Boosting Classifier was evaluated using Accuracy, Precision, Recall, and F1-score.

### Gradient Boosting Classification Results

| Class | Precision | Recall | F1-score | Support |
|---|---:|---:|---:|---:|
| 0 - No Purchase | 0.95 | 0.91 | 0.93 | 2055 |
| 1 - Purchase | 0.63 | 0.74 | 0.68 | 411 |
| **Accuracy** | | | **0.88** | **2466** |
| Macro Avg | 0.79 | 0.83 | 0.80 | 2466 |
| Weighted Avg | 0.89 | 0.88 | 0.89 | 2466 |

The Gradient Boosting Classifier reached **88.3% accuracy** on the test set.

---

## Business Insights

The analysis shows some clear differences between sessions that resulted in a purchase and those that did not.

The main insights are:

- Customers who viewed more product-related pages were more likely to make a purchase.
- Customers who spent more time on product pages also showed stronger purchase behavior.
- Higher `BounceRates` and `ExitRates` were more common in sessions without a purchase.
- `PageValues` was the most important feature in the prediction model.

These findings suggest that e-commerce businesses can focus on improving product page experience, encouraging deeper customer engagement, and reducing unnecessary website exits to support higher purchase intent.
