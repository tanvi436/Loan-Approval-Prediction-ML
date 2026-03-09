# Loan Approval Prediction using Machine Learning

## 📌 Project Overview

The **Loan Approval Prediction** project is a Machine Learning application that predicts whether a loan application will be approved or rejected based on applicant information such as income, credit history, education, marital status, property area, and employment status.

Financial institutions receive thousands of loan applications daily. Manually evaluating each application can be time-consuming and prone to human bias. This project aims to assist banks and financial organizations by using **Machine Learning algorithms to automate the loan approval process** and support decision-making.

The model analyzes applicant features and predicts the probability of loan approval.

---

## 🎯 Project Objective

The main objective of this project is to build a predictive machine learning model that can:

• Analyze applicant details
• Identify patterns affecting loan approval
• Predict whether a loan should be approved or rejected
• Improve decision-making efficiency for financial institutions

---

## 🗂 Dataset Description

The dataset used in this project contains applicant information and loan approval status.

### Dataset Features

| Feature           | Description                           |
| ----------------- | ------------------------------------- |
| Loan_ID           | Unique ID of loan application         |
| Gender            | Male / Female                         |
| Married           | Applicant marital status              |
| Dependents        | Number of dependents                  |
| Education         | Graduate / Not Graduate               |
| Self_Employed     | Self employed or not                  |
| ApplicantIncome   | Income of applicant                   |
| CoapplicantIncome | Income of co-applicant                |
| LoanAmount        | Loan amount requested                 |
| Loan_Amount_Term  | Loan repayment term                   |
| Credit_History    | Credit history of applicant           |
| Property_Area     | Rural / Semiurban / Urban             |
| Loan_Status       | Target variable (Approved / Rejected) |

---

## ⚙️ Technologies Used

The project is implemented using the following technologies:

**Programming Language**

• Python

**Libraries Used**

• Pandas – Data manipulation and analysis
• NumPy – Numerical computations
• Matplotlib – Data visualization
• Seaborn – Statistical visualization
• Scikit-learn – Machine learning modeling

---

## 🔄 Project Workflow

The project follows the complete machine learning pipeline:

### 1️⃣ Data Collection

The dataset containing loan application information is loaded using Pandas.

### 2️⃣ Data Preprocessing

Several preprocessing steps were performed:

• Handling missing values
• Data cleaning
• Removing unnecessary columns
• Handling inconsistent data

### 3️⃣ Handling Missing Values

Missing values were replaced using:

• Median values for numerical columns
• Mode values for categorical columns

### 4️⃣ Feature Encoding

Categorical features were converted into numerical format using mapping techniques.

Example:

Gender
Male → 1
Female → 0

Property Area
Rural → 0
Semiurban → 1
Urban → 2

### 5️⃣ Exploratory Data Analysis (EDA)

Data visualization was performed to understand relationships between variables.

Graphs created include:

• Loan Status Distribution
• Credit History vs Loan Approval
• Applicant Income Distribution
• Loan Amount Distribution
• Correlation Heatmap

These visualizations help identify patterns influencing loan approval.

### 6️⃣ Feature Selection

The target variable **Loan_Status** was separated from the input features.

```
X = df.drop("Loan_Status", axis=1)
y = df["Loan_Status"]
```

### 7️⃣ Train-Test Split

The dataset was split into training and testing sets.

• Training Data → 80%
• Testing Data → 20%

This ensures proper model evaluation.

### 8️⃣ Model Training

The machine learning model used:

**Logistic Regression**

Logistic Regression is suitable for **binary classification problems**, making it ideal for predicting loan approval status.

### 9️⃣ Model Evaluation

The model performance was evaluated using:

• Accuracy Score
• Confusion Matrix
• Classification Report

### 🔢 Model Accuracy

The model achieved an accuracy of:

**82.8%**

---

## 📊 Model Evaluation Metrics

### Confusion Matrix

The confusion matrix helps evaluate prediction performance by showing:

• True Positives
• True Negatives
• False Positives
• False Negatives

### Classification Report

The classification report provides:

• Precision
• Recall
• F1-score
• Support

These metrics help understand how well the model performs across different classes.

---

## 💾 Model Saving

The trained model was saved using **Joblib** so it can be reused later without retraining.

Example:

```
import joblib
joblib.dump(model, "loan_model.pkl")
```

---

## 📁 Project Structure

```
Loan-Approval-Prediction-ML
│
├── Loan_Prediction_Project.ipynb
├── loan_train.csv
├── loan_model.pkl
└── README.md
```

---

## 🚀 Applications

This project can be used in:

• Banking systems
• Financial institutions
• Loan approval automation systems
• Credit risk analysis
• FinTech applications

---

## 🔮 Future Improvements

The project can be improved further by:

• Using advanced machine learning models (Random Forest, XGBoost)
• Deploying the model using **Streamlit or Flask**
• Creating a web interface for real-time loan prediction
• Using larger and more complex datasets
• Performing feature engineering

---

## 👩‍💻 Author

Tanvi
Machine Learning & Data Science Enthusiast
