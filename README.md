# Fraud Detection in Financial Transactions using Machine Learning

This repository hosts a comprehensive end-to-end data science project focused on identifying fraudulent financial transactions. The project covers everything from Exploratory Data Analysis (EDA) to deploying a real-time prediction interface.

## 📌 Overview

Financial fraud represents a massive global challenge. This project leverages a large-scale synthetic dataset (over 6 million records) to build a robust classification model. It addresses critical data science hurdles such as **extreme class imbalance** and **feature pipeline automation**.

## 🚀 Tech Stack

* **Language:** Python 3.11+
* **Data Wrangling:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn (Logistic Regression, Pipelines, ColumnTransformer)
* **Deployment:** Streamlit
* **Model Serialization:** Joblib

## 📊 Project Workflow

1. **Exploratory Data Analysis (EDA):** Investigating transaction types, correlation matrices, and identifying patterns in balance discrepancies between origin and destination accounts.
2. **Feature Engineering:** Implementing `OneHotEncoder` for categorical variables and `StandardScaler` for numerical features to ensure model convergence.
3. **Handling Class Imbalance:** Utilizing the `class_weight='balanced'` parameter within the model to account for the fact that fraud represents only ~0.13% of the total dataset.
4. **Pipeline Architecture:** Building a Scikit-learn `Pipeline` to encapsulate preprocessing and modeling, ensuring consistency between training and inference.
5. **Web Application:** Developing an interactive dashboard using Streamlit for real-time fraud scoring based on user input.

## 🛠️ Installation & Usage

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/fraud-detection-ml.git

```


2. **Install dependencies:**
```bash
pip install -r requirements.txt

```


3. **Run the Streamlit app:**
```bash
streamlit run fraud_detection.py

```



## 📈 Performance & Results

The final model achieved an accuracy of **94%**. Key findings during the analysis highlighted that 'Transfer' and 'Cash Out' operations are the primary vectors for fraudulent activity, which guided the feature selection process.

---
