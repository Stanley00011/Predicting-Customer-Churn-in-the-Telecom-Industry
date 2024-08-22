# Predicting Customer Churn in the Telecom Industry

## Executive Summary
Customer churn is a critical issue for telecom companies, directly impacting revenue and customer lifetime value. This project analyzes customer data to predict churn, enabling proactive retention strategies. Using the Telco Customer Churn Dataset, we conducted thorough data exploration, built predictive models, and provided actionable recommendations.

## 1. Introduction
**Objective**: To predict customer churn in the telecom industry and generate insights for reducing churn rates.

**Dataset**: [Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn) from Kaggle.

## 2. Data Exploration and Cleaning
### Data Overview
- **Total Records**: 7,032 customers after cleaning
- **Key Attributes**: Customer demographics, service details, account information, churn status.

### Data Cleaning Steps
- **Convert `TotalCharges`** to numeric, handle errors.
- **Remove rows with missing `TotalCharges`** values.

## 3. Exploratory Data Analysis (EDA)
### Churn Distribution
![Churn Distribution](![churn dis](https://github.com/user-attachments/assets/9b7f143a-a79b-4a02-8aeb-a64b4d20788e)
)

**Insight**: Approximately 26% of customers have churned.

### Correlation Matrix
![Correlation Matrix](![cor mat](https://github.com/user-attachments/assets/f83691ec-5af1-4b6f-91d6-d97988d32121)
)

**Insight**: 
- **Tenure** has a strong negative correlation with churn.
- **MonthlyCharges** is positively correlated with churn.

### Feature Correlation with Churn
![Categorical Features with Churn](![cor of cat](https://github.com/user-attachments/assets/fbe9d792-f881-4b75-a871-761f8df48ba1)
)

**Key Insights**:
- **Contract type** (month-to-month) is highly correlated with churn.
- **Electronic check payment** method has a high churn rate.
- Customers without **tech support** or **online security** are more likely to churn.

## 4. Predictive Modeling
### Model Selection and Training
- **Model**: Gradient Boosting Classifier
- **Feature Scaling**: Applied standard scaling to numerical features.
- **Performance**: 
  - **Accuracy**: 80%
  - **Confusion Matrix** and **Classification Report** available in the project.

## 5. Recommendations
1. **Proactive Retention Strategy**:
   - Implement the Gradient Boosting model to identify and target high-risk customers.
   - Focus on customers with month-to-month contracts and high monthly charges for retention efforts.

2. **Incentivize Long-term Contracts**:
   - Offer discounts or benefits to customers who switch to long-term contracts.

3. **Enhanced Customer Support**:
   - Provide additional tech support and online security services, particularly to high-risk customers.

4. **Personalized Marketing Campaigns**:
   - Use insights from the model to create targeted campaigns aimed at retaining customers most likely to churn.

## 6. Conclusion
Predictive modeling and data-driven insights provide valuable strategies for reducing churn in the telecom industry. Implementing these recommendations can significantly improve customer retention and overall profitability.

## Visualizations
- Add the images generated during EDA to the `images` directory in your GitHub repository.
- Update the `path_to_image` with the correct relative paths to these images.

## How to Run the Code
- Ensure you have the required libraries installed: `pandas`, `seaborn`, `matplotlib`, `scikit-learn`.
- Place the dataset in the same directory as your script or adjust the `file_path` accordingly.
- Run the script to generate analysis, visualizations, and model outputs.
