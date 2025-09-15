
# Paisa Bazaar Project


This project aims to develop a machine learning pipeline to classify financial data into three categories: Good, Poor, and Standard. The goal is to provide actionable insights for business decisions, helping identify high-risk or high-value profiles effectively. The project leverages multiple ML models, hyperparameter tuning, and model evaluation to ensure optimal performance and real-world applicability.
## Project Summary

- **Objective:** 
    
    Build ML models to classify financial profiles for better decision-making and risk management.
- **Data Preprocessing:**

    - Handled class imbalance with resampling techniques.
    - Phone Number

    - Applied **Truncated SVD** for dimensionality reduction.

    - Encoded categorical target labels using Label Encoding.

- **Models Implemented:** 
    - Logistic Regression

    - Random Forest Classifier

    - XGBoost Classifier

- **Hyperparameter Optimization:**

    - Logistic Regression with BayesSearchCV

    - Random Forest with RandomizedSearchCV

    - XGBoost with RandomizedSearchCV

- **Evaluation Metrics:**
    
    Accuracy, Precision (macro), Recall (macro), F1-Score (macro), Confusion Matrix

- **Performance Summary:**

  
| Model                         | Accuracy | Precision | Recall | F1-Score |
| ----------------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression           | 0.64     | 0.63      | 0.68   | 0.64     |
| Optimized Logistic Regression | 0.83     | 0.82      | 0.81   | 0.82     |
| Random Forest                 | 0.79     | 0.77      | 0.80   | 0.78     |
| XGBoost                       | 0.73     | 0.71      | 0.73   | 0.72     |

- **Best Model:**

    Optimized Logistic Regression for its stability, interpretability, and improved performance metrics.

- **Model Deployment:**
    - Saved as ```best_model.pkl``` using joblib.

    - Capable of predicting unseen data; 
        
        sample output: ```['Standard', 'Standard', 'Good', 'Poor', 'Good']```

- **Business Impact:**
    - Improves decision-making and operational efficiency.

    - Identifies high-risk categories for proactive financial strategies.

    - Provides interpretable insights for stakeholders.
