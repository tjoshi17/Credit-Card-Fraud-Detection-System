# 💳 Credit Card Fraud Detection

## 📌 Understanding and Defining Fraud
Credit card fraud refers to any dishonest activity performed to gain unauthorized access to a cardholder’s financial information for monetary benefit.

One of the most common fraud techniques is **skimming**, where attackers duplicate data stored on the card’s magnetic stripe. Other common fraud methods include:

- Manipulation or alteration of genuine cards  
- Creation of counterfeit cards  
- Use of stolen or lost credit cards  
- Fraudulent telemarketing  

This project focuses on building a **machine learning model** to detect fraudulent transactions using historical transaction data.

---

## 📊 Data Understanding

The dataset used in this project is a simulated credit card transaction dataset from Kaggle, containing both legitimate and fraudulent transactions.

### 🔢 Dataset Summary:
- 👥 ~1,000 cardholders  
- 🏪 ~800 merchants  
- 📅 Time period: **1 Jan 2019 – 31 Dec 2020**  
- 📈 Total transactions: **1,852,394**  
- ⚠️ Fraudulent transactions: **9,651 (~0.52%)**  

### 🧾 Key Features:
- `amt` → Transaction amount  
- `is_fraud` → Target variable  
  - `1` → Fraudulent transaction  
  - `0` → Legitimate transaction  

⚠️ **Note:** The dataset is highly imbalanced, making fraud detection a challenging classification problem.

---

## ⚙️ Development Environment

Due to the large dataset size, the project is executed using:

- 📁 **Google Drive** → Data storage  
- 📓 **Google Colab** → Model development  

---

## 🔄 Project Pipeline

### 1️⃣ Understanding Data
- Load dataset  
- Explore features and data types  
- Identify relevant variables for modeling  

### 2️⃣ Exploratory Data Analysis (EDA)
- Perform **univariate & bivariate analysis**  
- Detect missing values and outliers  
- Handle skewness and apply transformations  

### 3️⃣ Train-Test Split
- Split dataset into training and testing sets  
- Use **Stratified K-Fold Cross Validation** to handle class imbalance  

### 4️⃣ Model Building & Hyperparameter Tuning
- Start with **baseline models (e.g., Logistic Regression)**  
- Experiment with advanced models:
  - Decision Trees  
  - Random Forest  
  - Gradient Boosting  
- Apply **sampling techniques**:
  - Oversampling (SMOTE)  
  - Undersampling  

### 5️⃣ Model Evaluation
Since the dataset is imbalanced, focus on fraud detection performance using:

- Precision  
- Recall  
- F1-Score  
- ROC-AUC  

🎯 **Business Goal:**  
Maximize the detection of fraudulent transactions (minimize false negatives), even at the cost of some false positives.

---

## 🚀 Objective

To build a robust and scalable fraud detection system that can accurately identify fraudulent transactions and minimize financial losses.
