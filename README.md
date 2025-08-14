# Loan Approval Prediction — Machine Learning Project

## Project Overview
This project develops a **predictive model** to determine **loan approval status** for applicants based on their demographic and financial details.  
The pipeline covers:
- Data cleaning & preprocessing
- Feature engineering
- Exploratory Data Analysis (EDA)
- Model training & evaluation

A **Support Vector Machine (SVM) classifier** was trained and achieved **81% accuracy** on the test dataset.

---

## Objectives
- Analyze factors influencing loan approval.
- Visualize trends and distributions in applicant data.
- Build and evaluate a machine learning model for approval prediction.
- Provide data-driven insights to support lending decisions.

---

## Dataset
- **Source**: Loan applicant dataset (similar to public domain datasets like Loan Prediction from Kaggle)  
- **Size**: ~1,000+ records  
- **Key Features**:
  - `Gender`, `Married`, `Dependents`, `Education`, `Self_Employed`
  - `ApplicantIncome`, `CoapplicantIncome`
  - `LoanAmount`, `Loan_Amount_Term`, `Credit_History`
  - `Property_Area`
  - `Loan_Status` (Target Variable)

---

## Project Workflow

### 1️⃣ Data Cleaning
- Handled missing values in categorical and numerical columns.
- Removed anomalies (e.g., negative income values).
- Standardized column names and formats.

### 2️⃣ Feature Engineering
- Label encoding for binary categorical features.
- One-hot encoding for nominal categorical variables.
- Created new features such as `Total_Income` and `EMI`.
- Normalized/standardized numerical features to improve SVM performance.

### 3️⃣ Exploratory Data Analysis
Visualizations built with **Matplotlib & Seaborn**:
- **Distribution plots** for applicant income & loan amount.
- **Bar charts** for loan approval rates by education, gender, and employment type.
- **Heatmap** for correlation between numerical features.
- **Boxplots** for income vs loan approval status.

### 4️⃣ Model Development
- Split the dataset into training and test sets (80:20).
- Tried multiple models (Logistic Regression, Decision Tree, Random Forest, SVM).
- Tuned hyperparameters for SVM (kernel, C, gamma) for optimal results.
- Evaluated performance using accuracy, confusion matrix, precision, recall, and F1-score.

---

## Results
- **Best Model**: Support Vector Machine (SVM) Classifier
- **Test Accuracy**: **81%**
- **Insights**:
  - Applicants with **Credit History = 1** had a significantly higher approval chance.
  - Higher total income is correlated with higher loan approval probability.
  - Self-employed applicants showed slightly lower approval rates.
  - Property area impacted approval, with **Semiurban** having the highest approvals.

---

## Tools & Technologies
| Tool / Library       | Purpose |
|----------------------|---------|
| **Python**           | Data analysis and modeling |
| **Pandas**           | Data manipulation |
| **NumPy**            | Numerical operations |
| **Matplotlib**       | Data visualization |
| **Seaborn**          | Statistical graphs |
| **Scikit-learn**     | Machine learning algorithms & preprocessing |
| **Google Collab** | Interactive development |

---

## Visualization Samples
<img width="1109" height="989" alt="download" src="https://github.com/user-attachments/assets/a1e88373-f010-4d5a-af9d-a56bcfb86eb1" />


---

