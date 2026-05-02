# 📊 Bank Marketing Prediction (End-to-End ML Project)

## 📌 Overview

This project presents a complete machine learning solution to predict whether a customer will subscribe to a term deposit based on bank marketing campaign data. The project includes data preprocessing, feature engineering, model building, and evaluation, with a strong focus on handling imbalanced data.

The final output is provided as an interactive HTML report.

---

## 🎯 Objective

* Predict customer subscription behavior (`yes` / `no`)
* Improve marketing campaign efficiency
* Support data-driven decision-making in banking

---

## 📂 Project Output

📄 **Final Report (HTML):**

* `Bankmarketing prediction.html` (interactive project report)

This report contains:

* Data analysis
* Visualizations
* Model results
* Business insights

---

## ⚙️ Project Workflow

### 🔹 Data Understanding

* Dataset: Bank Marketing Campaign Data
* Includes customer demographics, financial details, and campaign interactions

---

### 🔹 Data Preprocessing

* Handled missing values
* Encoded categorical variables
* Scaled numerical features
* Performed **train-test split before preprocessing** to avoid data leakage

---

### 🔹 Feature Engineering

* Created meaningful features such as:

  * Campaign effectiveness indicators
  * Customer interaction behavior
  * Derived ratios and grouped features

---

### 🔹 Handling Imbalanced Data

* Dataset contains significantly fewer positive cases (~11%)
* Applied:

  * SMOTE (oversampling technique)
  * Class balancing methods

---

### 🔹 Model Development

* Model Used: **Random Forest Classifier**
* Pipeline:

  * ColumnTransformer for preprocessing
  * Hyperparameter tuning using GridSearchCV
  * Cross-validation using StratifiedKFold

---

## 📊 Results

* **ROC-AUC:** ~0.91
* **Macro F1 Score:** ~0.74

### 🔍 Key Observations

* Accuracy is not reliable due to class imbalance
* F1-score and ROC-AUC provide better evaluation
* Model performs well in identifying potential subscribers

---

## 💡 Business Impact

* Helps target high-probability customers
* Reduces marketing costs
* Improves campaign conversion rates
* Enables data-driven marketing strategies

---

## 🛠 Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Imbalanced-learn (SMOTE)
* Matplotlib, Seaborn
* Jupyter Notebook

---

## 📁 Repository Structure

```id="9s8g7a"
bank-marketing-customer-prediction-ml/
│
├── report/
│   └── Bankmarketing prediction.html
│
├── notebook/ (optional)
│   └── .ipynb file
│
├── README.md
└── requirements.txt
```

---

## 🚀 How to Use

1. Download or clone this repository
2. Open the HTML file directly in your browser:

```id="k29x8q"
open "Bankmarketing prediction.html"
```

or simply double-click the file

---

## 📈 Key Learnings

* Built a complete ML pipeline from preprocessing to evaluation
* Applied techniques for handling imbalanced datasets
* Used feature engineering to improve predictive performance
* Translated model outputs into business insights

---

## 🇩🇪 Industry Relevance

This project reflects real-world use cases in:

* Banking and financial analytics
* Customer segmentation
* Marketing optimization
* Decision support systems used in German enterprises

---

## 👤 Author

**Priyaneiyah Selvakumar**
Master’s in Data Science & AI
📍 Berlin, Germany
💼 Open to Data Science / Machine Learning roles

---

## ⭐ Note

This project demonstrates practical machine learning implementation with business relevance and can be extended for real-time deployment.

