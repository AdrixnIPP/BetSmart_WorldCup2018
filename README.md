# Bets_Soccer_WorlCup2018
Analyse et modélisation prédictive pour un site de pari en ligne : Evaluation des performances des utilisateurs et prévision des comportements de paris en ligne.

```markdown
# LittleBigBet Data Analysis and Machine Learning Project

## Project Overview

This project is focused on analyzing the betting behavior of customers on the LittleBigBet platform, a football-focused online betting website. The goal of this project is to:

1. **Test the effectiveness** of a new feature that predicts match outcomes for premium users.
2. **Provide insights** through data analysis and suggest strategies for improving customer engagement.
3. **Develop predictive models** to forecast customer behavior, including the likelihood of a bet winning and the probability of a standard customer upgrading to a premium account.

## Datasets

We used three datasets for this analysis:

1. **bets.csv**: Contains detailed information about bets made on the platform.
2. **customers.csv**: Contains customer information, including whether they are premium users and if they had access to the new predictive service.
3. **pricing.csv**: Contains subscription pricing details for standard and premium users.

## Key Objectives

1. **Feature testing**: Analyze whether the new feature offered to premium users between June 14, 2018, and July 15, 2018, improved the betting experience.
2. **KPIs development**: Build a dashboard to monitor the company’s performance.
3. **Machine Learning**: Implement predictive models to forecast outcomes such as whether a customer will win a bet or upgrade to a premium account.

## Tools and Techniques Used

- **Data Preprocessing**: pandas, NumPy
- **Data Visualization**: Matplotlib, Seaborn
- **Machine Learning**: scikit-learn, RandomForestClassifier, LogisticRegression
- **Model Evaluation**: Accuracy, Precision, Recall, Confusion Matrix

## Folder Structure

```
├── data
│   ├── bets.csv
│   ├── customers.csv
│   ├── pricing.csv
├── notebooks
│   ├── 01_data_analysis.ipynb
│   ├── 02_machine_learning_models.ipynb
├── README.md
```

## Key Insights from the Analysis

1. **Customer behavior analysis**: There was no significant improvement in the win rate for customers who had access to the new service, indicating that the service did not significantly impact customer betting behavior.
2. **KPI Dashboard**: Monthly subscription trends and commission from bets were tracked to evaluate company performance.
3. **Machine Learning Models**:
   - **Prediction of Bet Outcome**: A Random Forest model was trained to predict whether a bet will win or lose based on the available features.
   - **Customer Conversion**: A Logistic Regression model was implemented to predict whether a standard customer will upgrade to a premium account.

## Machine Learning Models

### Model 1: Bet Outcome Prediction

The Random Forest model was trained using features such as the bet value, premium status, and test service access to predict the likelihood of a bet winning. The model achieved reasonable accuracy but could be further improved with more features and hyperparameter tuning.

### Model 2: Customer Premium Conversion

A Logistic Regression model was used to predict the likelihood of a customer upgrading from a standard account to a premium account. The model provides valuable insights into the factors that influence customer upgrades.
