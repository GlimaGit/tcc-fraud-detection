# tcc-fraud-detection
Financial fraud represents a massive global challenge. This project leverages a large-scale synthetic dataset (over 6 million records) to build a robust classification model. It addresses critical data science hurdles such as extreme class imbalance and feature pipeline automation.

🚀 Tech Stack
Language: Python 3.11+

Data Wrangling: Pandas, NumPy

Visualization: Matplotlib, Seaborn

Machine Learning: Scikit-learn (Logistic Regression, Pipelines, ColumnTransformer)

Deployment: Streamlit

Model Serialization: Joblib

📊 Project Workflow
Exploratory Data Analysis (EDA): Investigating transaction types, correlation matrices, and identifying patterns in balance discrepancies between origin and destination accounts.

Feature Engineering: Implementing OneHotEncoder for categorical variables and StandardScaler for numerical features to ensure model convergence.

Handling Class Imbalance: Utilizing the class_weight='balanced' parameter within the model to account for the fact that fraud represents only ~0.13% of the total dataset.

Pipeline Architecture: Building a Scikit-learn Pipeline to encapsulate preprocessing and modeling, ensuring consistency between training and inference.

Web Application: Developing an interactive dashboard using Streamlit for real-time fraud scoring based on user input.

🛠️ Installation & Usage
Clone the repository:

Bash

git clone https://github.com/your-username/fraud-detection-ml.git
Install dependencies:

Bash

pip install -r requirements.txt
Run the Streamlit app:

Bash

streamlit run fraud_detection.py
📈 Performance & Results
The final model achieved an accuracy of 94%. Key findings during the analysis highlighted that 'Transfer' and 'Cash Out' operations are the primary vectors for fraudulent activity, which guided the feature selection process.
