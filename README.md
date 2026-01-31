# Task 8: Decision Tree – Bank Marketing Subscription Prediction

## 📌 Overview

This project is part of the **AI & ML Internship – Task 8**. The objective is to build a **Decision Tree Classifier** to predict whether a customer will subscribe to a bank term deposit based on marketing campaign data. The task emphasizes **model interpretability**, **handling categorical data**, and **overfitting control**.

---

## 📂 Dataset

* **Source:** UCI / Kaggle Bank Marketing Dataset
* **Target Variable:** `y`

  * `yes` → Customer subscribed
  * `no` → Customer did not subscribe

The dataset contains customer demographic details, contact information, and past campaign outcomes.

---

## 🛠 Tools & Libraries Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib

---

## ⚙️ Steps Performed

### 1. Data Loading

* Loaded the Bank Marketing dataset using Pandas.
* Verified delimiter (`;`) and inspected dataset structure.

### 2. Data Cleaning

* Replaced `unknown` values with NaN.
* Filled missing values using **mode** for categorical consistency.

### 3. Feature Encoding

* Converted categorical features into numeric form using **Label Encoding**.
* Ensured all features were suitable for Decision Tree training.

### 4. Train-Test Split

* Split the dataset into training and testing sets (80:20).
* Used a fixed `random_state` for reproducibility.

### 5. Model Training

* Trained a **DecisionTreeClassifier**.
* Limited tree depth using `max_depth` to prevent overfitting.

### 6. Model Evaluation

* Compared **training accuracy vs testing accuracy** to detect overfitting.
* Generated a **classification report** (precision, recall, F1-score).

### 7. Tree Visualization

* Visualized the trained decision tree using `plot_tree()`.
* Saved the visualization as an image for submission.

### 8. Rule Extraction

* Interpreted the decision tree and derived **3 key decision rules** explaining customer subscription behavior.

---

## 🌳 Key Decision Rules (Example)

1. Customers with longer call duration are more likely to subscribe.
2. Customers with a successful outcome in a previous campaign have a high subscription probability.
3. Customers with very short call duration and no prior contact are unlikely to subscribe.

---

## 📊 Results

* Achieved reasonable test accuracy with controlled overfitting.
* Decision Tree provided clear and interpretable rules for business understanding.

---

## 📦 Deliverables

* Jupyter Notebook (`.ipynb`)
* Decision Tree visualization image
* Classification report
* README.md (this file)

---

## 🎯 Learning Outcome

* Gained hands-on experience with **Decision Trees**
* Understood **overfitting and depth control**
* Learned how to **interpret ML models using rules**

---

## 👤 Author

**Harsha**

AI & ML Internship
