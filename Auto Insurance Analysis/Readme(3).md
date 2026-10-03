# Auto Insurance Analysis

## 📌 Project Overview

This project analyzes customer data from an auto insurance company to
understand customer value, retention, churn patterns, and response to a
new insurance policy campaign.

The analysis focuses on **Customer Lifetime Value (CLV)**, customer
behavior, survival/retention patterns, and machine-learning models for
predicting CLV and campaign response.

------------------------------------------------------------------------

## 🎯 Objectives

-   Analyze customer characteristics and insurance policy information.
-   Understand factors associated with Customer Lifetime Value.
-   Identify customer segments contributing strongly to CLV.
-   Analyze customer retention and churn patterns over time.
-   Study customer response to a new policy advertisement.
-   Build machine-learning models for CLV prediction.
-   Build classification models for campaign-response prediction.
-   Generate business-oriented insights from the analysis.

------------------------------------------------------------------------

## 📊 Dataset

The project uses the **IBM Watson Marketing Customer Value Analysis**
dataset.

The dataset contains customer-level information such as:

-   Customer Lifetime Value
-   Response
-   Coverage
-   Education
-   Employment Status
-   Gender
-   Income
-   Location Code
-   Marital Status
-   Monthly Premium Auto
-   Months Since Last Claim
-   Months Since Policy Inception
-   Number of Open Complaints
-   Number of Policies
-   Policy Type
-   Policy
-   Renew Offer Type
-   Sales Channel
-   Total Claim Amount
-   Vehicle Class
-   Vehicle Size

### Dataset Size

-   **9,134 customer records**
-   **24 original columns**

------------------------------------------------------------------------

## 🛠️ Technologies Used

-   Python
-   Pandas
-   NumPy
-   Matplotlib
-   Seaborn
-   Scikit-learn
-   Jupyter Notebook

------------------------------------------------------------------------

## 🔄 Project Workflow

``` text
Data Loading
     ↓
Data Inspection
     ↓
Data Cleaning & Preparation
     ↓
Exploratory Data Analysis
     ↓
Customer Lifetime Value Analysis
     ↓
Customer Retention / Survival Analysis
     ↓
Campaign Response Analysis
     ↓
Feature Preparation
     ↓
Machine Learning
     ↓
Model Evaluation
     ↓
Business Insights
```

------------------------------------------------------------------------

## 🧹 Data Cleaning & Preparation

The analysis included:

-   Checking the dataset structure and data types.
-   Checking for missing values.
-   Removing columns that were not required for the modeling objective.
-   Converting categorical variables into appropriate categorical
    representations.
-   Separating numerical and categorical features.
-   Encoding categorical variables using one-hot encoding.
-   Scaling numerical features using `StandardScaler`.
-   Identifying and treating CLV outliers using the IQR method.

For CLV outlier treatment, values above:

``` text
Q3 + 1.5 × IQR
```

were treated as high outliers for the modeling analysis.

------------------------------------------------------------------------

## 📈 Exploratory Data Analysis

The project analyzes relationships between CLV and customer/policy
characteristics.

Areas investigated include:

-   CLV by policy type
-   CLV by vehicle class
-   CLV by coverage
-   CLV by employment status
-   CLV by education
-   CLV by gender
-   CLV by income
-   CLV by marital status
-   CLV by sales channel
-   CLV by vehicle size
-   Policy response patterns
-   Customer retention over time

------------------------------------------------------------------------

## 💰 Customer Lifetime Value Analysis

Customer Lifetime Value (CLV) represents the estimated value generated
by a customer during their relationship with the insurance company.

The analysis identifies customer and policy segments that contribute
significantly to overall CLV.

Some of the major segments observed in the analysis include:

-   Personal Auto -- Medsize
-   Corporate Auto -- Large
-   Personal Auto -- Large
-   Luxury vehicle segments

These findings can help an insurance company understand where customer
value is concentrated.

------------------------------------------------------------------------

## 🔁 Customer Retention & Survival Analysis

Customer retention was analyzed using:

-   Months Since Policy Inception
-   Number of customers stopping at each period
-   Retention rate
-   Hazard rate
-   Survival rate

### Key observation

The analysis shows relatively stable hazard patterns through
approximately the first 60 months, followed by an increase in the later
policy-inception periods.

This can help identify periods where additional customer-retention
strategies may be useful.

------------------------------------------------------------------------

## 🤖 Machine Learning

### 1. CLV Prediction

Regression models were compared to predict Customer Lifetime Value.

Models evaluated included:

-   Linear Regression
-   Ridge Regression
-   Lasso Regression
-   K-Nearest Neighbors
-   Support Vector Regression
-   Random Forest Regressor
-   Gradient Boosting Regressor

Evaluation metrics:

-   Mean Absolute Error (MAE)
-   Mean Squared Error (MSE)
-   R² Score

The analysis found that tree-based ensemble models performed strongly
for the CLV prediction task.

### 2. Campaign Response Prediction

Classification models were used to predict whether a customer would
respond to the new policy advertisement.

Models evaluated included:

-   Logistic Regression
-   Random Forest Classifier
-   Gradient Boosting Classifier
-   Support Vector Machine

Evaluation metrics:

-   Accuracy
-   Precision
-   Recall
-   F1 Score

Because campaign response is a classification problem, precision,
recall, and F1 score were considered in addition to accuracy.

------------------------------------------------------------------------

## 📊 Key Business Insights

-   Customer Lifetime Value varies considerably across policy and
    vehicle segments.
-   Personal Auto -- Medsize represents an important customer-value
    segment.
-   Some luxury vehicle segments contribute relatively high customer
    value.
-   Customer retention patterns change as the policy ages.
-   Campaign response differs across customer and policy segments.
-   Customer segmentation can help target marketing and retention
    campaigns.
-   CLV prediction can support prioritization of high-value customers.

------------------------------------------------------------------------

## 📁 Project Structure

``` text
Auto Insurance Analysis/
│
├── AutoInsuranceAnalysis.ipynb
├── CLV_contribution.png
├── CLV_hist.jpg
├── hazard_survival_churn_analysis.png
├── Response.png
│
├── data/
│   └── WA_Fn-UseC_-Marketing-Customer-Value-Analysis.csv
│
├── .gitignore
└── Readme.md
```

------------------------------------------------------------------------

## ▶️ How to Run the Project

### 1. Clone the repository

``` bash
git clone https://github.com/Nabisha40/auto-insurance-analysis.git
```

### 2. Open the project

``` bash
cd auto-insurance-analysis
```

### 3. Install required libraries

``` bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Start Jupyter Notebook

``` bash
jupyter notebook
```

Open:

``` text
AutoInsuranceAnalysis.ipynb
```

and run the notebook cells.

------------------------------------------------------------------------

## 📌 Project Attribution

This repository is being maintained as a learning and portfolio project.

The project files were obtained from an existing GitHub source, but the
original repository/author has not yet been identified. The source
should be added here once identified.

**Original source:** To be updated after verification.

Any future modifications or additional analysis will be documented
separately.

------------------------------------------------------------------------

## ⚠️ Note

The machine-learning results shown in the notebook should be interpreted
as an analysis of the available dataset, not as guaranteed production
performance.

In particular, unusually high classification performance should be
validated for possible data leakage, overfitting, class imbalance, and
other modeling issues before deployment.

------------------------------------------------------------------------

## 👤 Author

**Nabisha40**

GitHub:\
https://github.com/Nabisha40
