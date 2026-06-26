# 💳 Financial Fraud Analysis using Machine Learning

> **End-to-end financial fraud analysis using exploratory data analysis, feature engineering, and machine learning to identify fraudulent financial transactions and generate actionable business insights.**

---

# 📖 Overview

Financial fraud is a significant challenge for banks and digital payment platforms, leading to financial losses, operational risks, and reduced customer trust.

This project presents an end-to-end machine learning workflow for analyzing financial transaction data, discovering fraud patterns through exploratory data analysis (EDA), and developing a predictive model capable of distinguishing fraudulent transactions from legitimate ones.

The project demonstrates practical data science skills, including data preprocessing, visualization, feature engineering, class imbalance handling, machine learning, and model evaluation.

---

# 🎯 Project Objectives

* Analyze historical financial transaction data.
* Identify fraud trends using exploratory data analysis.
* Perform data preprocessing and feature engineering.
* Handle imbalanced classification problems.
* Build a machine learning model for fraud detection.
* Generate meaningful business insights from transaction data.

---

# 📊 Dataset Overview

The dataset consists of synthetic financial transaction records containing customer information, merchant details, transaction metadata, and fraud labels.

**Problem Type**

* Binary Classification

**Target Variable**

* `is_fraud`

Each transaction is labeled as:

* **0** → Legitimate Transaction
* **1** → Fraudulent Transaction

---

# 🔑 Dataset Features

| Feature               | Description                 |
| --------------------- | --------------------------- |
| trans_date_trans_time | Transaction timestamp       |
| cc_num                | Masked credit card number   |
| merchant              | Merchant name               |
| category              | Merchant category           |
| amt                   | Transaction amount          |
| first, last           | Customer name               |
| gender                | Customer gender             |
| city, state           | Customer location           |
| lat, long             | Customer coordinates        |
| merch_lat, merch_long | Merchant coordinates        |
| city_pop              | Population of customer city |
| job                   | Customer occupation         |
| dob                   | Date of birth               |
| trans_num             | Transaction ID              |
| unix_time             | Unix timestamp              |
| is_fraud              | Fraud Label                 |

---

# 🏗️ Project Workflow

```
Financial Transaction Dataset
            │
            ▼
      Data Cleaning
            │
            ▼
 Exploratory Data Analysis
            │
            ▼
 Feature Engineering
            │
            ▼
 Handling Class Imbalance
            │
            ▼
 Machine Learning Model
            │
            ▼
 Model Evaluation
            │
            ▼
 Business Insights
```

---

# 📁 Repository Structure

```
financial-fraud-analysis/

├── data/
│   └── fraudTest.csv
│
├── images/
│   ├── fraud_count_by_gender.png
│   ├── fraud_rate_by_gender.png
│   ├── top10_cities_fraud.png
│   └── top10_states_fraud.png
│
├── notebooks/
│   └── financial_fraud_analysis.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

# 🔍 Exploratory Data Analysis

The exploratory data analysis focuses on understanding fraud behavior across customer demographics, transaction characteristics, and geographic regions.

Key analyses include:

* Transaction distribution
* Fraud class imbalance
* Fraud count by gender
* Fraud rate by gender
* Top fraud-prone states
* Top fraud-prone cities
* Transaction amount analysis
* Correlation analysis

---

# 📈 Key Findings

* The dataset is highly imbalanced, with legitimate transactions significantly outnumbering fraudulent ones.
* Fraudulent transactions exhibit distinct transaction amount patterns.
* Fraud occurrence varies across geographic regions.
* Certain cities and states experience comparatively higher fraud frequencies.
* Customer demographic analysis reveals differences in fraud distribution across gender.

---

# 🤖 Machine Learning Pipeline

The predictive modeling workflow includes:

* Data Cleaning
* Feature Engineering
* Categorical Encoding
* Handling Class Imbalance
* Train-Test Split
* Random Forest Classification
* Model Evaluation

Future versions will compare multiple machine learning models including:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

---

# 🛠️ Tech Stack

### Programming

* Python

### Data Analysis

* Pandas
* NumPy

### Data Visualization

* Matplotlib
* Seaborn

### Machine Learning

* Scikit-learn
* imbalanced-learn

### Development Environment

* Jupyter Notebook

---

# ⚙️ Installation

```bash
git clone https://github.com/ROCKYBH7/financial-fraud-analysis.git

cd financial-fraud-analysis

pip install -r requirements.txt

jupyter notebook notebooks/financial_fraud_analysis.ipynb
```

---

# 🚀 Future Improvements

* Compare multiple machine learning models.
* Apply SMOTE for oversampling.
* Perform hyperparameter tuning.
* Add ROC and Precision-Recall curves.
* Deploy the trained model using FastAPI or Streamlit.
* Build an interactive fraud analytics dashboard.

---

# 👨‍💻 Author

**Balaji R H**

**AI Engineer | Machine Learning Engineer | Generative AI Developer**

📧 [balajirh.ds@gmail.com](mailto:balajirh.ds@gmail.com)

💼 LinkedIn: https://www.linkedin.com/in/balaji-r-h-a81107298

🐙 GitHub: https://github.com/ROCKYBH7

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
