# 🕵️‍♂️ Fraud Detection Project

This repository contains a complete end-to-end **fraud detection** analysis using a synthetic transaction dataset. The goal is to identify fraudulent transactions through data exploration, preprocessing, visualization, and machine learning classification.

---

## 📁 Repository Structure

```
Fraud_Detection_Project/
├── fraud_detection.ipynb             # Jupyter notebook with EDA & ML pipeline
└── README.md                         # Project documentation
```

---

## 📦 Dataset Overview

The dataset contains transaction records with 22 features and a binary label indicating fraud. Each row represents one transaction.

## 🔑 Key Features

| Feature              | Description                                               |
|----------------------|-----------------------------------------------------------|
| `trans_date_trans_time` | Date and time of the transaction                      |
| `cc_num`             | Credit card number (masked)                               |
| `merchant`           | Merchant name                                             |
| `category`           | Merchant category                                         |
| `amt`                | Transaction amount                                        |
| `first`, `last`      | Cardholder’s first and last name                          |
| `gender`             | Gender of the cardholder (`M` / `F`)                      |
| `street`, `city`, `state`, `zip` | Cardholder’s address                        |
| `lat`, `long`        | Latitude and Longitude of cardholder’s location           |
| `city_pop`           | Population of the cardholder’s city                       |
| `job`                | Cardholder’s job title                                    |
| `dob`                | Date of birth                                             |
| `trans_num`          | Unique transaction ID                                     |
| `unix_time`          | Unix timestamp of the transaction                         |
| `merch_lat`, `merch_long` | Merchant’s geographical coordinates              |
| `is_fraud`           | Target column (`1`: Fraud, `0`: Not Fraud)                |


---

## 🔍 Exploratory Data Analysis (EDA)

Key insights obtained from EDA:

- ✅ No null values in the dataset.
- 📊 Imbalanced target: Majority of transactions are **not fraud**.
- 👩‍🦰 Gender-based analysis: Female fraud rate higher in some regions.
- 🌆 Fraud distribution by **state** and **city** highlighted key fraud-prone areas.
- 💰 Fraud transactions mostly involve amounts > $200.
- 📌 Visuals:
  - Countplots of fraud by gender
  - Fraud distribution by state
  - Boxplots of amount vs. fraud
  - Heatmaps for correlation analysis

---

## 🧪 Preprocessing & Modeling

- ✅ Dropped irrelevant features: `dob`, `trans_num`, `unix_time`, etc.
- 🧼 Encoded categorical variables using `LabelEncoder` and `get_dummies`.
- 📉 Handled **class imbalance** with `RandomUnderSampler`.
- 🧠 Model used: **Random Forest Classifier**
- ✅ Train-Test Split: 80-20
- ⚙️ Evaluation Metrics: Accuracy, Precision, Recall, F1-score

---

## 📈 Results Summary

```
   precision    recall  f1-score   support

           0       0.75      0.75      0.75         4
           1       0.75      0.75      0.75         4

    accuracy                           0.75         8
   macro avg       0.75      0.75      0.75         8
weighted avg       0.75      0.75      0.75         8
```

> ⚠️ Note: The small test size (8 samples) limits generalizability. Cross-validation and hyperparameter tuning are recommended for better performance.

---

## 💡 Future Improvements

- Apply **SMOTE** for synthetic oversampling.
- Try **XGBoost** or **LightGBM** for better performance.
- Deploy model with **Flask** or **Streamlit**.
- Automate model training with ML pipelines.

---

## 🧰 Tech Stack

- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- imbalanced-learn (for under-sampling)
- Jupyter Notebook

---

## 📦 Installation

```bash
# Clone the repo
git clone https://github.com/ROCKYBH7/Fraud_Detection_Project.git
cd Fraud_Detection_Project

# Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook fraud_detection.ipynb
```
---

## 👤 Author

**Balaji R H**  
📧 balajirh.ds@gmail.com  
🔗 LinkedIn: linkedin.com/in/balaji-r-h-a81107298  
🐙 GitHub: github.com/ROCKYBH7  

---

## 📝 License

This project is licensed under the MIT License - feel free to use and adapt it.

---

## ⭐️ Show your support

If you found this project helpful, consider giving it a ⭐️ on GitHub!
