# <font face = 'Palatino Linotype' color = '#5885AF'> Employee Productivity Prediction with Machine Learning<font/>

## 📌 Project Overview
Employee productivity is a critical driver of organizational success. This project aims to develop a predictive machine learning model that estimates an employee’s ProductivityScore using demographic, performance, and engagement-related data provided by the Human Resources and Development department. By identifying key factors that influence productivity, this project supports data-driven workforce management, improved performance strategies, and better organizational decision-making.

## 🎯 Business Objective
Management seeks to gain deeper insight into the drivers of employee productivity across the organization. The primary objective is to:
Develop a predictive model that accurately estimates employee productivity based on key individual and work-related characteristics.

## The insights generated from this model can help the organization:
- Improve workforce management and employee development strategies
- Optimize training programs and performance reviews
- Support data-driven decisions in promotions, hiring, and resource allocation
- Enhance overall organizational efficiency and employee satisfaction

## 🗂 Dataset Description
The dataset includes a comprehensive set of employee attributes, such as:
- Demographic Information: Age, education level, department, tenure
- Work Structure: Remote work ratio, work hours, project load
- Engagement & Feedback: Job satisfaction, managerial feedback
- Career Development: Training participation, promotion history
- Performance Indicators: Recent performance ratings

### Target Variable:
ProductivityScore

## 🤖 Machine Learning Models Used

The following regression models were implemented and evaluated:
- Lasso Regression
- Ridge Regression
- Elastic Net Regression
- Random Forest Regressor
All models were trained and evaluated using cross-validation, with performance measured primarily by Root Mean Squared Error (RMSE).

## 📈 Model Evaluation & Results
Cross-Validation Performance (RMSE)
- Elastic Net Regression and Lasso Regression demonstrated the most promising performance, achieving the lowest CV RMSE among all models.
- Elastic Net Regression emerged as the best-performing model overall.

### Why Elastic Net?
- Elastic Net Regression was selected as the final model because:
- Its CV RMSE closely matched its training RMSE, indicating no signs of overfitting
- It generalized well to unseen test data
- It effectively balances feature selection (L1 regularization) and coefficient stability (L2 regularization)
This makes Elastic Net particularly suitable for datasets with correlated predictors and mixed feature importance.

## ✅ Key Takeaways
Regularized linear models performed better than more complex models for this dataset
Elastic Net provided the best balance between bias, variance, and interpretability
Productivity is influenced by a combination of engagement, workload, and performance-related features
The model provides actionable insights that can directly inform HR and management policies
