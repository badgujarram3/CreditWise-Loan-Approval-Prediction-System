# 💳 CreditWise: Loan Approval Prediction System

### Machine Learning | Exploratory Data Analysis | Feature Engineering | Classification

CreditWise is a machine learning project designed to analyze loan applicants' financial and personal information and predict whether their loan applications are likely to be approved.

The project follows an end-to-end machine learning workflow, including data exploration, data cleaning, visualization, categorical encoding, feature engineering, model training, and evaluation.

Multiple classification algorithms are compared to identify a suitable model for predicting loan approval outcomes.

---

## 📌 Project Overview

Financial institutions need to evaluate several factors before approving a loan, including applicant income, credit score, existing financial obligations, savings, collateral value, and loan amount.

CreditWise uses these features to learn patterns from historical loan application data and generate predictions for new applicants.

### 🎯 Project Objectives

* Understand the loan approval dataset through exploratory data analysis (EDA).
* Identify patterns and relationships between applicant characteristics and loan approval.
* Clean and prepare the dataset for machine learning.
* Visualize numerical and categorical features.
* Encode categorical variables into machine-readable formats.
* Perform feature engineering to improve the quality of input features.
* Analyze feature relationships using a correlation heatmap.
* Split the data into training and testing sets.
* Train and evaluate multiple classification models.
* Compare models using appropriate classification metrics.
* Identify the best-performing model based on precision.
* Predict loan approval outcomes for new applicants.

---

## 📂 Dataset Description

The dataset contains **950 applicant records and 20 columns**, based on the initial dataset inspection.

It includes applicant demographics, income details, credit information, existing liabilities, loan characteristics, and the historical loan approval outcome.

### Dataset Features

| Feature            | Description                                          |
| ------------------ | ---------------------------------------------------- |
| Applicant_ID       | Unique applicant identifier                          |
| Applicant_Income   | Income of the applicant                              |
| Coapplicant_Income | Income of the co-applicant                           |
| Employment_Status  | Applicant's employment status                        |
| Age                | Applicant's age                                      |
| Marital_Status     | Marital status                                       |
| Dependents         | Number of dependents                                 |
| Credit_Score       | Applicant's credit score                             |
| Existing_Loans     | Number of existing loans                             |
| DTI_Ratio          | Debt-to-income ratio                                 |
| Savings            | Applicant's savings                                  |
| Collateral_Value   | Estimated value of collateral                        |
| Loan_Amount        | Requested loan amount                                |
| Loan_Term          | Duration of the requested loan                       |
| Loan_Purpose       | Purpose of the loan                                  |
| Property_Area      | Applicant's property area category                   |
| Education_Level    | Applicant's education level                          |
| Gender             | Applicant's gender                                   |
| Employer_Category  | Category of the applicant's employer                 |
| Loan_Approved      | Historical loan approval outcome and target variable |

**Target variable:** `Loan_Approved`

The target represents the historical approval outcome. Its actual values and class distribution should be checked before model training.

*Note: Dataset descriptions and units should be verified against the original data source.*

---

## 🛠️ Technologies Used

* **Programming Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn
* **Development Environment:** Jupyter Notebook

### Machine Learning Algorithms

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Gaussian Naive Bayes

---

## 🔄 Project Workflow

The project follows a structured machine learning pipeline.

## 🔄 Project Workflow

1. **Dataset Loading and Understanding**
2. **Exploratory Data Analysis (EDA)**
3. **Data Cleaning and Preprocessing**
4. **Data Visualization**
5. **Categorical Feature Encoding**
6. **Correlation Analysis and Heatmap**
7. **Feature Engineering**
8. **Train-Test Split**
9. **Machine Learning Model Training**
   * Logistic Regression
   * K-Nearest Neighbors (KNN)
   * Gaussian Naive Bayes
10. **Model Evaluation and Performance Comparison**
11. **Best Model Selection Based on Precision**
12. **Loan Approval Prediction for New Applicants**


---

## 📊 Model Evaluation

The trained models should be evaluated using multiple metrics rather than relying on accuracy alone.

| Evaluation Metric | Purpose                                                      |
| ----------------- | ------------------------------------------------------------ |
| Accuracy          | Proportion of correctly classified applications              |
| Precision         | Proportion of predicted approvals that are actually approved |
| Recall            | Proportion of actual approvals correctly identified          |
| F1-score          | Harmonic mean of precision and recall                        |

For this project, **precision is an important model comparison metric**, as the objective includes evaluating how reliably the model identifies applications belonging to the predicted approval class.

However, loan approval is a high-impact financial decision. False rejections and false approvals can both have significant consequences. Therefore, precision should be interpreted alongside recall, the confusion matrix, and the costs of different types of errors.

### Best Model Selection

Based on the model comparison performed in the project, Gaussian Naive Bayes is the reported best-performing model for precision.

The actual evaluation results should be added below after confirming them from the notebook.

| Model                |    Accuracy |   Precision |      Recall |    F1-score |
| -------------------- | ----------: | ----------: | ----------: | ----------: |
| Logistic Regression  | To be added | To be added | To be added | To be added |
| KNN                  | To be added | To be added | To be added | To be added |
| Gaussian Naive Bayes | To be added | To be added | To be added | To be added |


---

## 🔮 Loan Approval Prediction

Once the model is trained, it can be used to generate predictions for new applicants.

The input information may include:

* Applicant and co-applicant income.
* Employment status.
* Age and number of dependents.
* Credit score.
* Existing loans.
* Debt-to-income ratio.
* Savings.
* Collateral value.
* Requested loan amount.
* Loan term and purpose.
* Property area.
* Education level.
* Gender and employer category.

The applicant's information must be transformed using the same preprocessing steps used during training.

### Prediction Output

The model can return a predicted class:

* **Likely Approved:** The model predicts the approval class.
* **Likely Not Approved:** The model predicts the non-approval class.

If the trained model supports probability estimates, the project may also display the estimated probability associated with the predicted class.

A predicted probability is not a guaranteed approval chance. It should not be presented as a reliable real-world probability unless the model has been appropriately validated and calibrated.

---

## 💡 Key Learning Outcomes

Through this project, I practiced:

* Exploratory data analysis using Pandas.
* Data cleaning and preprocessing.
* Numerical and categorical data visualization.
* Categorical feature encoding.
* Correlation analysis using heatmaps.
* Feature engineering.
* Train-test splitting and leakage prevention.
* Training multiple classification algorithms.
* Comparing classification metrics.
* Evaluating precision, recall, and F1-score.
* Applying a trained model to new applicant information.
* Organizing a machine learning project for GitHub.

---

## 📁 Project Structure

```text
CreditWise-Loan-Approval-Prediction/
│
├── data/
│   └── loan_approval.csv
│
├── notebooks/
│   └── CreditWise_Loan_Approval_Prediction.ipynb
│
├── Visual insights/
│
├── models/
│
├── README.md
```

The folder structure is a recommendation. Include only files that exist in your project. If you save the trained model, add the actual model file and the corresponding loading or inference code.

---

## 👨‍💻 Author

**Ram Sanjay Badgujar**

B.Tech Data Science Engineering Student

Interested in Data Science, Machine Learning, Data Analytics, and Data Engineering.

* **GitHub:** https://github.com/badgujarram3
* **LinkedIn:** https://www.linkedin.com/in/ram-badgujar-5a8b48335/

---