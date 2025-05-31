# Customer-Churn-Prediction-ML-DL
End-to-end customer churn prediction using classical machine learning and deep learning models. Includes EDA, feature engineering, SMOTE balancing, model tuning (LogReg, RF, XGBoost), and deep learning with MLP and TabNet — all focused on actionable business insights.

A complete churn prediction pipeline using structured customer data — from exploratory analysis to model deployment. This project combines classical ML and deep learning (MLP, TabNet) to build interpretable and high-performing retention models that support real-world business decisions.



## 🚀 Model Comparison Summary

This project evaluates several models for customer churn prediction. Below is a performance comparison:

| Model                  | Accuracy | Recall | Precision | ROC AUC |
|------------------------|----------|--------|-----------|---------|
| Logistic Regression    | 79%      | 0.12   | 0.32      | 0.65    |
| Logistic + SMOTE       | 82%      | 0.68   | 0.38      | 0.75    |
| Random Forest          | 82%      | 0.43   | 0.44      | 0.74    |
| XGBoost                | 83%      | 0.41   | 0.48      | 0.74    |
| MLP (Deep Learning)    | 82%      | 0.39   | 0.47      | 0.77    |
| TabNet (Deep Learning) | 82%      | 0.40   | 0.49      | 0.77    |

> These results support strategic churn reduction, enabling data-driven decisions aligned with business goals.

## 💼 Final Business Insights

1. **Churn Detection is Now Actionable**  
   The baseline logistic regression model had limited recall (0.12), making it ineffective at detecting churners. After applying **SMOTE**, recall improved drastically (to **0.68**). Advanced models like **Random Forest**, **XGBoost**, and deep learning methods (**MLP** and **TabNet**) delivered recall in the **0.39–0.43** range with higher AUC scores, making predictions significantly more usable for retention planning.

2. **Model Selection Should Reflect Business Strategy**  
   - **Logistic Regression + SMOTE** gave the **highest recall (0.68)** and is ideal for wide-net retention outreach.  
   - **XGBoost** offered the best trade-off between **precision (0.48)** and **recall (0.41)**, suited for campaigns targeting fewer but high-risk customers.  
   - **Random Forest** balanced solid recall (0.43) with **interpretability**, a great fit for business stakeholders.  
   - **Deep Learning Models**:
     - **MLP (Multilayer Perceptron)** achieved strong classification performance with an **AUC of 0.77**, suitable for capturing non-linear churn patterns.  
     - **TabNet**, a deep learning model optimized for tabular data, also delivered an **AUC of 0.77** with high interpretability — allowing transparent, accurate churn prediction.

3. **Age is the Most Influential Churn Driver**  
   All models — including TabNet’s built-in feature attribution — identified **Age** as the top predictor. This enables targeted retention strategies like proactive engagement for older users or personalized incentives.

4. **Behavioral Metrics Matter**  
   Key behavioral features like **Credit Score**, **Tenure**, and **Balance** were strong churn indicators across both ML and DL models. These can be used to define high-risk customer personas.

5. **Data-Led Retention Strategy is Now Viable**  
   With AUC scores up to **0.77**, precision and recall in actionable ranges, and feature explainability from both ML and DL models, the business can now confidently **segment and retain at-risk customers** — maximizing customer lifetime value through informed, data-driven strategies.
