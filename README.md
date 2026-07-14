# Banking-Credit-Risk-Classification
An end-to-end machine learning project for multi-class customer priority classification using statistical analysis, exploratory data analysis, feature engineering, XGBoost, and model explainability to support data-driven banking decisions.

# 🏦 Banking Credit Risk Prediction

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Classification-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

An end-to-end Machine Learning project that predicts customer credit risk by analyzing demographic, financial, and behavioral attributes. The project includes comprehensive data preprocessing, exploratory data analysis, feature engineering, model comparison, hyperparameter tuning, and business-driven evaluation to help financial institutions identify high-risk customers and support better lending decisions.

---

# 📑 Table of Contents

- [🏦 Project Overview](#-project-overview)
- [💼 Business Problem](#-business-problem)
- [🎯 Objectives](#-objectives)
- [📂 Dataset](#-dataset)
- [✨ Project Features](#-project-features)
- [🛠 Tech Stack](#-tech-stack)
- [🔄 Project Workflow](#-project-workflow)
- [📁 Repository Structure](#-repository-structure)

---

# 🏦 Project Overview

Financial institutions process thousands of loan applications every day. Approving loans for customers who are likely to default increases financial losses, while rejecting reliable customers reduces business opportunities.

This project develops a Machine Learning solution capable of predicting customer credit risk using historical banking data. By analyzing customer demographics, financial history, account information, and behavioral patterns, the model classifies customers into different risk categories, enabling banks to make faster and more informed lending decisions.

---

# 💼 Business Problem

Banks must evaluate loan applicants before approving credit.

Manual risk assessment can be:

- Time-consuming
- Subjective
- Inconsistent
- Difficult to scale

The objective is to build a predictive model that accurately identifies customers with higher credit risk, helping banks reduce defaults while improving the loan approval process.

---

# 🎯 Objectives

- Understand customer characteristics through exploratory data analysis.
- Identify important financial and demographic predictors.
- Handle missing values and categorical variables.
- Reduce multicollinearity where necessary.
- Train multiple classification models.
- Compare model performance.
- Optimize the best-performing model.
- Predict customer credit risk accurately.

---

# 📂 Dataset

| Attribute | Description |
|-----------|-------------|
| Domain | Banking |
| Problem Type | Multi-Class Classification |
| Target Variable | Customer Credit Risk Profile |
| Features | Customer Demographics, Financial Information, Behavioral Variables |
| Data Format | CSV |
| Industry | Banking & Financial Services |

---

# ✨ Project Features

| Module | Description |
|---------|-------------|
| Data Preprocessing | Cleaning, missing value treatment, encoding |
| Exploratory Data Analysis | Statistical analysis & visualization |
| Feature Selection | Important predictor identification |
| Multicollinearity Analysis | VIF evaluation |
| Model Training | Multiple ML classification models |
| Hyperparameter Tuning | Model optimization |
| Performance Evaluation | Accuracy, Precision, Recall, F1-score |
| Business Interpretation | Risk-based decision making |

---

# 🛠 Tech Stack

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, XGBoost |
| Statistical Analysis | Statsmodels |
| Model Evaluation | Accuracy, Precision, Recall, F1-score |
| Development Environment | Jupyter Notebook |

---

# 🔄 Project Workflow

```text
Raw Banking Dataset
          │
          ▼
Data Cleaning
          │
          ▼
Feature Engineering
          │
          ▼
Exploratory Data Analysis
          │
          ▼
Feature Selection
          │
          ▼
Multicollinearity Check
          │
          ▼
Model Training
          │
          ▼
Hyperparameter Tuning
          │
          ▼
Model Evaluation
          │
          ▼
Credit Risk Prediction
```

---

# 📁 Repository Structure

```text
Banking-Credit-Risk-Prediction/
│
├── data/
│
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_eda.ipynb
│   ├── 04_model_building.ipynb
│
├── models/
│
├── images/
│
├── requirements.txt
│
└── README.md
```

# 🧹 Data Preprocessing

The raw banking dataset contained missing values, categorical variables, class imbalance, and features with varying scales. A structured preprocessing pipeline was developed to transform the raw data into a clean, machine-learning-ready dataset while preserving important customer and financial information.

---

# 🎯 Objectives

- Handle missing values appropriately
- Clean inconsistent records
- Encode categorical variables
- Prepare numerical features for modeling
- Detect multicollinearity
- Build a robust dataset for classification

---

# ⚙️ Data Preprocessing Pipeline

| Step | Description |
|------|-------------|
| Import Dataset | Load the banking dataset using Pandas |
| Data Inspection | Examine shape, data types, duplicates, and missing values |
| Missing Value Treatment | Handle null values using appropriate imputation techniques |
| Duplicate Removal | Remove repeated customer records |
| Feature Transformation | Convert categorical variables into numerical representations |
| Feature Scaling | Normalize numerical variables where required |
| Train-Test Split | Split data for unbiased model evaluation |
| Export Processed Data | Save the cleaned dataset for model development |

---

# 📊 Data Quality Assessment

| Assessment | Purpose |
|------------|---------|
| Dataset Shape | Understand dataset dimensions |
| Data Types | Verify numerical and categorical features |
| Missing Values | Identify incomplete observations |
| Duplicate Records | Prevent biased learning |
| Summary Statistics | Analyze distributions and detect anomalies |

---

# 🔄 Missing Value Strategy

Different preprocessing techniques were applied depending on the feature type.

| Feature Type | Strategy |
|-------------|----------|
| Numerical Variables | Median or Mean Imputation |
| Categorical Variables | Mode Imputation |
| Invalid Records | Removed only when necessary |
| Duplicate Entries | Completely removed |

---

# 🔤 Categorical Feature Encoding

Since machine learning models cannot directly process text-based variables, categorical features were transformed into numerical representations.

| Encoding Technique | Application |
|-------------------|-------------|
| Label Encoding | Ordinal categorical variables |
| One-Hot Encoding | Nominal categorical variables |
| Binary Representation | Yes/No attributes |

---

# 📈 Exploratory Data Analysis (EDA)

EDA was performed to understand customer characteristics, identify important predictors, detect patterns, and uncover business insights before model development.

---

# 🎯 Objectives of EDA

- Understand customer demographics
- Analyze financial characteristics
- Study relationships between predictors and target classes
- Detect outliers
- Identify important variables
- Support feature selection

---

# 📊 Univariate Analysis

Each feature was analyzed independently to understand its distribution.

## Numerical Features

| Feature | Purpose |
|----------|----------|
| Age | Customer demographics |
| Income | Financial capacity |
| Loan Amount | Credit exposure |
| Credit Score | Customer reliability |
| Existing Loans | Financial obligations |

---

## Categorical Features

| Feature | Business Importance |
|----------|---------------------|
| Occupation | Income stability |
| Education | Financial profile |
| Marital Status | Customer segmentation |
| Employment Status | Repayment capability |
| Residential Status | Financial stability |

---

# 📈 Distribution Analysis

The following visualizations were used throughout EDA.

| Visualization | Purpose |
|--------------|---------|
| Histogram | Distribution analysis |
| Boxplot | Outlier detection |
| Countplot | Frequency comparison |
| Bar Chart | Category comparison |
| Pie Chart | Class proportions |
| Heatmap | Correlation analysis |

---

# 🎯 Target Variable Analysis

The target variable was analyzed to understand class distribution and potential imbalance.

| Analysis | Purpose |
|----------|---------|
| Class Frequency | Distribution of risk categories |
| Percentage Distribution | Business interpretation |
| Class Balance | Identify imbalance before modeling |

The case study predicts multiple customer risk profiles, making it a **multi-class classification** problem. :contentReference[oaicite:0]{index=0}

---

# 🔍 Bivariate Analysis

Relationships between individual predictors and the target variable were examined to identify influential features.

### Numerical Features vs Target

| Feature | Relationship |
|----------|-------------|
| Credit Score | Strong |
| Annual Income | Moderate |
| Loan Amount | Strong |
| Existing Loans | Moderate |
| Age | Moderate |

### Categorical Features vs Target

| Feature | Business Insight |
|----------|------------------|
| Occupation | Certain professions showed different risk profiles |
| Education | Education level influenced repayment behaviour |
| Employment | Stable employment reduced default risk |
| Residential Status | Home ownership indicated stronger financial stability |
| Marital Status | Showed varying repayment patterns |

---

# 📊 Top Predictive Features

The importance of individual variables was assessed to understand which customer characteristics contribute most to credit risk prediction.

| Feature Category | Business Contribution |
|------------------|----------------------|
| Financial Features | Very High |
| Credit History | Very High |
| Income Variables | High |
| Employment Information | High |
| Customer Demographics | Moderate |

---

# 📉 Correlation Analysis

Correlation analysis was performed to identify relationships among numerical variables and detect redundant information.

| Objective | Benefit |
|-----------|---------|
| Detect highly correlated variables | Reduce redundancy |
| Improve interpretability | Easier business explanation |
| Support feature selection | Better model performance |

---

# 📐 Multicollinearity Analysis (VIF)

Variance Inflation Factor (VIF) was used to evaluate multicollinearity among numerical predictors.

### Why VIF?

- Detect redundant variables
- Improve model stability
- Reduce coefficient variance
- Improve interpretability

The case study also notes that performing **parallel VIF checks** is not an appropriate approach, emphasizing careful interpretation of multicollinearity analysis. :contentReference[oaicite:1]{index=1}

---

# 💼 Business Insights

EDA generated several valuable insights for banking decision-making.

| Finding | Business Value |
|----------|----------------|
| Financial variables strongly influence credit risk | Better lending decisions |
| Credit history remains one of the strongest predictors | Improved customer assessment |
| Employment information contributes significantly | Better borrower profiling |
| Customer demographics provide additional context | Improved segmentation |
| Some predictors are highly correlated | Supports feature reduction |

---

# 🚀 Key Outcomes

- ✅ Cleaned and standardized banking dataset
- ✅ Handled missing values effectively
- ✅ Encoded categorical variables for machine learning
- ✅ Identified influential customer characteristics
- ✅ Performed multicollinearity assessment using VIF
- ✅ Generated actionable business insights
- ✅ Prepared the dataset for classification model development

---

# 📌 Conclusion

The preprocessing and exploratory data analysis stages transformed raw banking data into a structured, high-quality dataset suitable for machine learning. Statistical analysis and business insights helped identify the most influential predictors of customer credit risk, providing a strong foundation for feature selection, model training, and predictive analytics.

# ⚙️ Feature Engineering

Feature engineering transformed raw customer information into meaningful predictors that improved the classification model's ability to distinguish between different customer risk profiles. Domain knowledge from the banking sector was combined with statistical techniques to create a robust feature set while reducing redundancy.

---

# 🎯 Objectives

- Improve predictive performance
- Reduce redundant information
- Increase model interpretability
- Create machine-learning-ready features
- Identify the most informative predictors

---

# 🔄 Feature Engineering Workflow

```text
Clean Dataset
      │
      ▼
Feature Transformation
      │
      ▼
Categorical Encoding
      │
      ▼
Feature Selection
      │
      ▼
Multicollinearity Analysis
      │
      ▼
Final Feature Set
```

---

# 🔧 Feature Transformation

Several preprocessing and transformation techniques were applied before model training.

| Technique | Purpose |
|-----------|---------|
| Categorical Encoding | Convert text into numerical format |
| Missing Value Imputation | Preserve valuable observations |
| Feature Scaling | Standardize numerical variables |
| Feature Selection | Remove less informative predictors |
| VIF Analysis | Detect multicollinearity |

---

# 📊 Feature Importance Analysis

Feature importance analysis was performed to understand which variables contribute most to customer credit risk prediction.

| Feature Category | Business Importance |
|------------------|---------------------|
| Credit History | Very High |
| Financial Information | Very High |
| Loan Information | High |
| Income Variables | High |
| Customer Behaviour | Moderate |
| Demographics | Moderate |

The analysis showed that only a subset of variables contributes significantly to predicting customer risk, allowing less informative features to be removed before model training.

---

# 📉 Feature Selection

Feature selection was performed to improve model performance and reduce unnecessary complexity.

### Objectives

- Remove noisy features
- Reduce overfitting
- Improve model interpretability
- Reduce training time

---

# 📌 Feature Selection Techniques

| Technique | Purpose |
|-----------|---------|
| Correlation Analysis | Remove redundant variables |
| Feature Importance | Rank influential predictors |
| Statistical Analysis | Identify significant variables |
| VIF Analysis | Remove multicollinearity |

---

# 📐 Multicollinearity Check

Highly correlated predictors can negatively affect certain machine learning models.

Variance Inflation Factor (VIF) was used to evaluate relationships among numerical variables.

| VIF Value | Interpretation |
|-----------|---------------|
| < 5 | Low Multicollinearity |
| 5–10 | Moderate |
| >10 | High |

Reducing multicollinearity improves model stability and makes feature importance easier to interpret.

---

# 🤖 Model Development

Multiple classification algorithms were trained and evaluated to identify the best-performing model for predicting customer credit risk.

---

# 🔄 Machine Learning Pipeline

```text
Processed Dataset
        │
        ▼
Train-Test Split
        │
        ▼
Feature Selection
        │
        ▼
Model Training
        │
        ▼
Hyperparameter Tuning
        │
        ▼
Performance Evaluation
        │
        ▼
Final Model
```

---

# 🧠 Classification Models Evaluated

| Model | Description |
|--------|-------------|
| Logistic Regression | Baseline linear classifier |
| Decision Tree | Rule-based classification |
| Random Forest | Ensemble of decision trees |
| XGBoost | Gradient boosting classifier |

Each model was evaluated using identical train-test splits to ensure a fair comparison.

---

# 📊 Evaluation Metrics

Several classification metrics were used because accuracy alone does not fully represent model performance.

| Metric | Purpose |
|---------|----------|
| Accuracy | Overall prediction performance |
| Precision | Correct positive predictions |
| Recall | Ability to identify actual positives |
| F1-Score | Balance between Precision and Recall |
| Confusion Matrix | Class-wise prediction analysis |

---

# 📈 Model Comparison

| Model | Strengths | Limitations |
|--------|-----------|-------------|
| Logistic Regression | Simple and interpretable | Limited nonlinear capability |
| Decision Tree | Easy to understand | Can overfit |
| Random Forest | Robust and accurate | Higher computational cost |
| XGBoost | Excellent predictive performance | Requires hyperparameter tuning |

---

# ⚙️ Hyperparameter Tuning

After comparing baseline models, the best-performing model was further optimized.

The tuning process focused on improving:

- Generalization
- Prediction accuracy
- Class-wise performance
- Model robustness

Parameters optimized included:

- Learning Rate
- Maximum Depth
- Number of Estimators
- Subsample Ratio
- Column Sampling
- Regularization Parameters

---

## 🏆 Final Model Selection

After evaluating multiple classification algorithms, **XGBoost** was selected as the final model because it provided the best balance between predictive accuracy and generalization.

According to the case study, XGBoost was chosen for further fine-tuning after comparative evaluation. It also highlighted that one risk class remained more difficult to predict, indicating opportunities for future feature engineering and model improvements. :contentReference[oaicite:0]{index=0}

---

## 📉 Confusion Matrix Interpretation

The confusion matrix was used to evaluate predictions for each customer risk category.

It helped identify:

- Correct classifications
- Misclassified customers
- Difficult-to-predict classes
- Areas requiring model improvement

---

## 📊 Business Interpretation

| Business Question | ML Solution |
|-------------------|-------------|
| Which customers are high risk? | Classification Model |
| Which features influence risk? | Feature Importance Analysis |
| Which model performs best? | Model Comparison |
| How reliable are predictions? | Evaluation Metrics |
| How can lending decisions improve? | Risk Classification |

---

## 🚀 Key Outcomes

- ✅ Built multiple classification models
- ✅ Compared algorithm performance
- ✅ Applied feature selection techniques
- ✅ Evaluated multicollinearity using VIF
- ✅ Optimized the best-performing model
- ✅ Selected XGBoost for final prediction
- ✅ Generated interpretable business insights

---

## 📈 Model Performance Summary

| Metric | Result |
|---------|--------|
| Problem Type | Multi-Class Classification |
| Final Algorithm | XGBoost |
| Model Selection | Based on comparative evaluation |
| Final Accuracy | **79.9%** |

---

## 💼 Business Impact

The developed machine learning solution enables financial institutions to:

- Identify high-risk customers before loan approval
- Improve consistency in credit risk assessment
- Reduce potential loan defaults
- Support faster and more informed lending decisions
- Enhance overall portfolio risk management

---

## 📌 Conclusion

This project demonstrates a complete end-to-end banking machine learning pipeline, from data preprocessing and exploratory analysis to feature engineering, model comparison, and predictive modeling. By leveraging statistical analysis and advanced ensemble learning techniques, the final XGBoost model provides an effective framework for customer credit risk classification and supports data-driven decision-making in the banking sector.

## 🏆 Project Results

The developed machine learning pipeline successfully classified customers into different credit risk profiles using demographic, financial, and behavioral information. Multiple classification algorithms were evaluated, and the final optimized model demonstrated strong predictive performance for banking risk assessment.

---

## 📊 Performance Summary

| Metric | Result |
|---------|--------|
| Problem Type | Multi-Class Classification |
| Final Model | XGBoost Classifier |
| Evaluation Metric | Accuracy |
| Final Accuracy | **79.9%** |
| Model Selection | Best performing after hyperparameter tuning |

---

## 📈 Key Achievements

- ✅ Built an end-to-end banking machine learning pipeline.
- ✅ Cleaned and preprocessed customer financial data.
- ✅ Performed comprehensive exploratory data analysis.
- ✅ Identified the most influential customer risk factors.
- ✅ Reduced multicollinearity using statistical analysis.
- ✅ Compared multiple machine learning algorithms.
- ✅ Optimized the XGBoost model through hyperparameter tuning.
- ✅ Achieved **79.9% classification accuracy**.
- ✅ Generated business-oriented insights for credit risk assessment.

---

## 💼 Business Impact

The developed solution provides several advantages for financial institutions.

| Business Challenge | Machine Learning Solution |
|--------------------|--------------------------|
| Manual credit assessment | Automated risk prediction |
| Slow loan approval process | Faster decision support |
| Higher default risk | Early identification of risky applicants |
| Inconsistent evaluation | Standardized ML-driven predictions |
| Portfolio risk management | Better customer segmentation |

---

## 📊 Business Insights

The project revealed several important findings:

- Financial attributes are the strongest predictors of customer credit risk.
- Customer credit history significantly influences repayment behavior.
- Employment and income stability improve creditworthiness.
- Some customer classes remain difficult to predict, indicating opportunities for richer feature engineering and additional data collection.
- Ensemble learning models outperform traditional linear classifiers for this problem.

---

## 📷 Project Screenshots

> Store all screenshots inside the **images/** folder.

```md
## Dashboard

![Dashboard](images/dashboard.png)

## Data Distribution

![EDA](images/eda.png)

## Feature Importance

![Feature Importance](images/feature_importance.png)

## Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

## Model Performance

![Model Comparison](images/model_comparison.png)
```

---

## ⚡ Installation

## Clone Repository

```bash
git clone https://github.com/<your-username>/banking-credit-risk-prediction.git
```

## Navigate to Project

```bash
cd banking-credit-risk-prediction
```

## Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Launch Jupyter Notebook

```bash
jupyter notebook
```

---

## 📦 Requirements

| Library | Purpose |
|----------|---------|
| Pandas | Data manipulation |
| NumPy | Numerical computing |
| Matplotlib | Visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning |
| XGBoost | Gradient Boosting |
| Statsmodels | Statistical analysis |
| SciPy | Scientific computing |
| Jupyter Notebook | Development Environment |

---

## 📖 What I Learned

Through this project, I gained practical experience in:

- Banking domain analytics
- Credit risk modeling
- Multi-class classification
- Data preprocessing techniques
- Feature engineering
- Statistical analysis
- Exploratory Data Analysis
- Feature selection
- Multicollinearity analysis (VIF)
- Hyperparameter tuning
- Ensemble learning using XGBoost
- Model evaluation and interpretation

---

# 🔮 Future Improvements

- Deploy the model using **Streamlit** or **FastAPI**.
- Handle class imbalance using **SMOTE** or class weighting.
- Build an explainable AI dashboard using **SHAP** values.
- Integrate real-time banking APIs for automated risk assessment.
- Experiment with **LightGBM** and **CatBoost**.
- Monitor model drift and retrain periodically with new customer data.
- Implement an end-to-end MLOps pipeline for production deployment.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork this repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

## Faraz Syed

**Aspiring Data Scientist | M.Sc. Statistics**

### Connect with Me

- 💼 LinkedIn: https://www.linkedin.com/in/faraz-syed-9786ba2aa/
- 💻 GitHub:https://github.com/sdFARAZ?tab=repositories
- 📧 Email: farazsyedx@gmail.com

---

## ⭐ If you found this project useful...

Please consider giving it a **Star ⭐** on GitHub.
