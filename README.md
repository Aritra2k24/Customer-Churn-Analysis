# 📊 Customer Churn Analysis Using Python & SQLite

## 📌 Project Overview

Customer churn is a critical business problem where customers stop using a company's products or services. Understanding the factors associated with churn can help businesses improve customer retention, identify high-risk customers, and reduce revenue loss.

This project performs an end-to-end **Customer Churn Analysis** using **Python, Pandas, SQLite3, Matplotlib, and Seaborn**. The analysis combines customer information, subscription details, and customer support interactions to identify churn patterns, calculate key business KPIs, and generate actionable business insights.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Clean and preprocess customer-related datasets.
- Integrate customer, subscription, and customer support data.
- Perform feature engineering to create meaningful analytical features.
- Calculate important customer churn and revenue KPIs.
- Analyze churn across plans, states, subscription types, and customer characteristics.
- Identify potential churn-risk indicators.
- Visualize churn trends and relationships between important variables.
- Generate business-oriented insights to support customer retention strategies.

---

## 🗂️ Dataset

The project uses a **SQLite customer churn database** containing three relational tables:

### 1. Customer

Contains customer-level information such as customer ID, demographic details, location, and other customer attributes.

### 2. Subscription

Contains information related to customer subscriptions, plans, contracts, tenure, revenue, and churn status.

### 3. Customer Support

Contains customer support interaction information such as complaints and escalations.

The three tables were loaded into **Pandas DataFrames** for data cleaning, transformation, and analysis.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Data analysis and preprocessing |
| Pandas | Data cleaning, transformation, and analysis |
| NumPy | Numerical operations |
| SQLite3 | Database connection and SQL queries |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Development and analysis |

---

## 🔄 Project Workflow

### 1. Data Loading

The customer churn database was connected using Python's `sqlite3` library. The three tables — `customer`, `subscription`, and `customer_support` — were loaded into Pandas DataFrames for further processing.

### 2. Data Cleaning & Preprocessing

The datasets were inspected and cleaned to improve data quality and consistency.

Key preprocessing activities included:

- Handling missing values.
- Removing unnecessary columns.
- Renaming columns with meaningful names.
- Converting columns to appropriate data types.
- Standardizing inconsistent categorical values.
- Checking data consistency.
- Preparing the datasets for analysis.

### 3. Feature Engineering

New analytical features were created using existing customer, subscription, and support attributes.

Examples include:

- Churn risk indicators
- Churn flags
- Churn scores
- Customer tenure features
- Complaint-related features
- Escalation-related features
- Revenue-related metrics
- Customer support activity metrics

### 4. Data Integration

The three datasets were joined using appropriate customer identifiers to create an integrated analytical dataset.

This allowed customer information, subscription behavior, revenue, complaints, escalations, and churn status to be analyzed together.

---

# 📈 Key Performance Indicators (KPIs)

The project calculates several business-oriented KPIs, including:

### Customer Metrics

- Number of unique customers
- Number of unique customers with complaints
- Average customer tenure
- Average complaints per user
- Average Revenue Per User (ARPU)

### Churn Metrics

- Overall churn rate
- Retention rate
- Churn by plan type
- Churn by state
- Churn by subscription type
- Churn risk analysis
- Revenue lost from churned customers

### Customer Support Metrics

- Complaint rate
- Escalation rate
- Average complaints per user
- Correlation between escalations and churn

### Revenue Metrics

- Total revenue
- Revenue by state
- Customer count by state
- Revenue lost due to churn

---

# 📊 Data Visualization

Several visualizations were created using **Matplotlib and Seaborn** to identify customer behavior and churn patterns.

### Visualizations include:

- 📈 Monthly Churn Trend
- 📊 Churn by Plan Type
- 📍 Churn by State
- 📊 Churn by Subscription Type
- 📈 Churn Risk Analysis
- 🔥 Correlation Analysis
- 📊 Churn Score vs. Churn Flag
- 📊 Escalations vs. Churn
- 📊 Contract Type Analysis
- 🔍 Pairplot for feature relationships
- 📊 Catplot for categorical analysis
- 📋 Pivot tables for summarized business analysis

---

# 🔍 Key Analysis Areas

The analysis focuses on answering questions such as:

- Which subscription plans have higher churn rates?
- Which states have higher customer churn?
- How does subscription type influence churn?
- What percentage of customers are retained?
- How much revenue is associated with churned customers?
- Do customers with more complaints have a higher likelihood of churn?
- Is there a relationship between support escalations and customer churn?
- Which customer groups represent higher churn risk?
- How does customer tenure relate to churn behavior?

---

# 💡 Business Value

The analysis can help businesses:

- Identify customer segments with higher churn rates.
- Monitor churn trends over time.
- Identify customers showing potential churn-risk indicators.
- Understand the relationship between customer support issues and churn.
- Estimate revenue associated with churned customers.
- Compare customer retention across subscription plans and regions.
- Develop targeted customer retention strategies.

---

# 📁 Project Structure

```text
Customer-Churn-Analysis/
│
├── data/
│   └── customer_churn.db
│
├── notebook/
│   └── Customer_Churn_Analysis.ipynb
│
├── visualizations/
│   ├── monthly_churn_trend.png
│   ├── churn_by_plan.png
│   ├── churn_by_state.png
│   └── ...
│
├── README.md
└── requirements.txt
