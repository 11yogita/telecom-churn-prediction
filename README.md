telecom-churn-prediction
Machine learning project to predict telecom customer churn using XGBoost, SMOTE and SHAP, with a Streamlit app for real-time risk scoring.

# PROBLEM STATEMENT 
Identify the telecom customers who are likely to churn, so that the company can target them with retention offers, thus reducing revenue loss.

# BUSINESS CCONTEXT 
It costs significantly more to win a new customer than to retain an existing one. Early identification of high-risk customers enables the business to act before they leave.

# Success Metrics
- Primary: Recall on the churn class.
  Missing a real churner is the costliest Mistake, since that customer is lost without any retention     attempt.
- Secondary: ROC-AUC.
  Measures how well the model separates churners from non-churners across all thresholds.
- Also tracked: Precision and F1-score,
  to avoid wasting retention offers on customers who would have stayed anyway.
- Not used as the main metric: Accuracy.
  Only ~26% of customers churn, so a model that predicts "no churn" for everyone would still score       ~74% accuracy while being useless.
