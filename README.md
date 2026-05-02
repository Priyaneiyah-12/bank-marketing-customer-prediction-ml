# 📊 Bank Marketing Customer Prediction (Machine Learning)

## 📌 Overview

This project develops an end-to-end machine learning pipeline to predict whether a customer will subscribe to a term deposit based on direct marketing campaign data. The solution focuses on handling class imbalance, building robust predictive models, and translating results into actionable business insights.

---

## 🎯 Business Objective

Marketing campaigns often suffer from low conversion rates and high operational costs. This project aims to:

* Identify high-probability customers
* Optimize campaign targeting
* Reduce unnecessary outreach efforts
* Improve return on investment (ROI)

---

## 📂 Dataset

* Source: UCI Bank Marketing Dataset
* Records: ~45,000 customer entries
* Features: Demographic, financial, and campaign-related attributes
* Target Variable: Subscription (`yes` / `no`)

---

## ⚙️ Methodology

### 🔹 1. Data Preprocessing

* Performed **train-test split before preprocessing** to avoid data leakage
* Handled missing values:

  * Numerical → Median Imputation
  * Categorical → Most Frequent Imputation
* Scaled numerical features using **StandardScaler**
* Encoded categorical variables using **OneHotEncoder (drop='first')**

---

### 🔹 2. Feature Engineering

Created domain-driven features to improve model performance:

* `campaign_success` → identifies effective contact frequency
* `recent_contact` → captures recency of interaction
* `age_group` → categorizes customer segments
* `duration_age` → interaction feature for behavioral insight

---

### 🔹 3. Handling Class Imbalance

The dataset is highly imbalanced (~11% positive class).
Applied:

* **SMOTE (Synthetic Minority Oversampling Technique)**
* Compared with **class_weight balancing**

---

### 🔹 4. Model Development

* Model: **Random Forest Classifier**
* Pipeline built using **ColumnTransformer**
* Hyperparameter tuning with **GridSearchCV**
* Cross-validation using **StratifiedKFold**

---

## 📊 Results

| Metric   | Score |
| -------- | ----- |
| ROC-AUC  | ~0.91 |
| Macro F1 | ~0.74 |

### ✅ Key Insights

* Accuracy alone is misleading due to class imbalance
* Macro F1 and ROC-AUC provide better evaluation
* SMOTE improved minority class detection

---

## 💡 Business Impact

* Enables **data-driven marketing decisions**
* Reduces campaign costs by targeting the right customers
* Improves customer conversion rates
* Supports scalable decision-making in banking and CRM systems

---

## 🛠 Tech Stack

* **Programming:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn
* **ML Techniques:** Random Forest, SMOTE, GridSearchCV
* **Visualization:** Matplotlib, Seaborn
* **Tools:** Jupyter Notebook / Google Colab

---

## 📁 Project Structure

```
bank-marketing-customer-prediction-ml/
│
├── notebook/
│   └── M505B_GH1050210.ipynb
│
├── report/
│   └── M505B_GH1050210.html
│
├── data/ (optional)
│   └── bank-additional-full.csv
│
├── README.md
├── requirements.txt
```

---

## 🚀 How to Run

### 🔹 1. Clone Repository

```
git clone https://github.com/yourusername/bank-marketing-customer-prediction-ml.git
cd bank-marketing-customer-prediction-ml
```

### 🔹 2. Install Dependencies

```
pip install -r requirements.txt
```

### 🔹 3. Run Notebook

```
jupyter notebook
```

---

## 📈 Key Learning Outcomes

* Built a complete **ML pipeline from scratch**
* Applied **feature engineering for business relevance**
* Handled **imbalanced datasets effectively**
* Performed **model tuning and evaluation using proper metrics**
* Translated technical results into **business insights**

---

## 🇩🇪 Industry Relevance (Germany)

This project demonstrates skills aligned with:

* Predictive analytics in banking & finance
* Customer segmentation and targeting
* Decision-support systems used in German enterprises
* End-to-end ML pipelines for real-world applications

---

## 🔗 Project Output

* 📄 Full Report: `report/M505B_GH1050210.html`
* 📓 Notebook: `notebook/M505B_GH1050210.ipynb`

---

## 👤 Author

**Priyaneiyah Selvakumar**
Master’s in Data Science & AI (Germany)
📍 Berlin, Germany
💼 Open to Data Science / ML roles

---

## ⭐ If You Like This Project

Feel free to ⭐ the repository and connect with me!
