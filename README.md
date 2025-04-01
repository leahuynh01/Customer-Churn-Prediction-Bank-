# Customer Churn Prediction for Bank
## Business Problem
Customer churn is a critical issue for Bank, leading to revenue loss, low customer engagement and increased acquisition costs. This project aims to predict customer churn by identifying key factors influencing retention and enabling businesses to take proactive measures.

## Business Questions
- Which customers are most likely to churn?
- What are the key drivers of customer churn?
- How can the company optimize retention strategies to reduce churn?
- What is the expected revenue impact if churn is reduced?

## Data Overview & Preparation Steps
### Data Overview
The dataset contains customer demographics, account information, and usage patterns. Key features include:
- Demographics: Age, gender, geography
- Account Details: Tenure, number of products, credit score, balance
- Behavioral Factors: Transactions, activity levels.

### Data Collection
The dataset was sourced from public datasets.
https://www.kaggle.com/datasets/mervetorkan/churndataset

### Data Preparation & Feature Engineering
- Preprocessing: Handling missing values, encoding categorical variables, scaling numerical features.
- Feature Engineering: Creating new variables such as balance per estimatedSalary.

## Methodologies
### Tools: 
Python, Pandas, NumPy, Scikit-learn, Tensorflow, Matplotlib, Seaborn

### Techniques:
- Machine Learning Models: Support Vector Machine (SVM), Gradient Boosting (LightGBM, GXBoost), Deep Learning (Sequential Model)
- Feature Selection: Using Boruta for selecting the most important predictors and Heatmap
- Hyperparameter Tuning: Using GridSearchCV for model optimization
- Model Evaluation: Cross-validation with StratifiedKFold, precision-recall analysis

## Results


Baseline Model: Logistic Regression achieved ~65% accuracy

Optimized Model: LightGBM achieved ~78% accuracy, 71% precision, and 76% recall

Business Impact: With targeted retention strategies, the company can reduce churn by 10-15%, potentially increasing revenue retention by $X million.

Reproducibility: The entire pipeline is documented, and models are saved in the models folder for future use.

## Growth & Next Steps
- Implement the trained model as an API or within a business dashboard.
- Provide marketing and customer service teams with churn risk scores for proactive engagement.
- Test different retention strategies based on the model’s predictions (A/B Testing)