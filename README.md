# phase3_project

**SYRIATEL CUSTOMER CHURN PREDICTION**

**OVERVIEW**

Customer churn is a major challenge in the telecommunications industry, leading to significant revenue loss. The objective of this project is to build a predictive model that identifies customers at high risk of churning so that SyriaTel can take proactive retention actions.

**BUSINESS AND DATA UNDERSTANDING** 

The primary stakeholder for this project is the Customer Retention Manager at SyriaTel, who is responsible for minimizing churn and improving customer satisfaction.

**BUSINESS PROBLEM** 

SyriaTel experiences customer attrition, which directly impacts revenue. The company needs a way to proactively identify customers who are likely to churn so that preventive actions (e.g., promotions, improved support) can be taken.

**DATASET**

The dataset contains 3,333 customer records with features such as:

- Account information (e.g., account length)

- Service plans (e.g., international plan, voicemail plan)

- Usage behavior (calls, minutes, charges)

- Customer service interactions

The target variable is churn, indicating whether a customer left the service.

**MODELING** 

An iterative modeling approach was used:

1. Baseline Model

Logistic Regression - Chosen for its simplicity and interpretability

2. Improved Models

Tuned Logistic Regression (hyperparameter tuning)

Decision Tree Classifier (nonparametric model)

**Approach:**

Data was split into training and testing sets.

Preprocessing included:

- Encoding categorical variables.

- Scaling numerical features (where appropriate).

- Care was taken to avoid data leakage by fitting transformations only on training data. 

**EVALUATION**

**Key Metric: Recall**

Recall was selected as the primary metric because:

- The goal is to identify as many churners as possible

- Missing a churner results in lost revenue

**Model Performance (Summary)**

The final model achieved strong recall, meaning it successfully identified a high proportion of at-risk customers.

Trade-off: Some false positives were present, but acceptable given the business context. 

**Key Insights**

- Customers with frequent customer service calls are more likely to churn.

- High usage customers may be more sensitive to service quality.

- Certain service plans influence churn likelihood.

**CONCLUSION**

This project demonstrates that machine learning can effectively predict customer churn using historical data. The final model provides actionable insights that can help SyriaTel reduce customer attrition.

**RECOMMENDATIONS** 

- Target customers with high customer service interactions for proactive engagement.

- Improve customer support quality to reduce dissatisfaction.

- Offer incentives or retention packages to high-risk customers.

- Monitor high-usage customers closely, as they represent valuable accounts.

**NEXT STEPS**

- Deploy the model into a real-time customer monitoring system.

- Continuously retrain the model with updated data.

- Experiment with more advanced models (e.g., Random Forest, Gradient Boosting).

- Conduct A/B testing on retention strategies.
