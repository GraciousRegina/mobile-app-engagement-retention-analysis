# Mobile App User Engagement & Retention Analysis

## Overview
This project analyzes mobile app user behavior across onboarding, activation, engagement, retention, subscription conversion, and revenue. It combines product analytics, cohort analysis, A/B testing, statistical inference, and machine learning.

## Dataset
This project uses a **synthetic dataset of 20,000 mobile app users** created to simulate realistic product engagement, onboarding, retention, subscription, and experimentation patterns. It is for portfolio demonstration and does not represent users from a real company.

## Key Results
- Onboarding completion: 72.83%
- Activation rate: 60.51%
- Day 7 retention: 46.06%
- Day 30 retention: 40.90%
- Subscription rate: 14.56%
- 30-day revenue: $86,599.97
- Activated-user D30 retention: 56.41% vs 17.13% for non-activated users
- Strongest cohort/channel combination: February 2026 / Organic at 43.14% D30 retention

## A/B Testing
A simulated Control/Treatment experiment was evaluated using two-proportion z-tests and 95% confidence intervals.

The Treatment onboarding experience increased completion from **69.96% to 75.65%**:
- Absolute lift: +5.69 percentage points
- Relative lift: +8.13%
- 95% CI: [4.45, 6.92] percentage points
- Statistically significant at the 5% level

Improvements in activation, Day 7 retention, Day 30 retention, and subscription were not statistically significant.

## Retention Prediction
Logistic Regression and Random Forest were compared for predicting Day 30 retention.

**Best model: Logistic Regression**
- ROC-AUC: 0.7918
- F1 score: 0.6601
- Recall: 0.6235
- High-risk users identified: 7,527

Random Forest feature importance identified Day 7 retention as the strongest predictor, followed by activation and feature usage.

## Business Recommendations
1. Adopt the improved onboarding experience while monitoring downstream outcomes.
2. Make activation a primary product KPI.
3. Focus retention interventions during the first week.
4. Improve feature discovery and product education.
5. Target high-risk users with re-engagement strategies.
6. Evaluate acquisition channels using downstream retention, not only signup volume.
7. Continue experiments focused on activation, retention, and subscription.

## Tools & Methods
Python, pandas, NumPy, Matplotlib, scikit-learn, SciPy, statsmodels, Google Colab, funnel analysis, cohort analysis, A/B testing, hypothesis testing, confidence intervals, Logistic Regression, Random Forest, ROC-AUC, feature importance, and retention-risk segmentation.

## Project Structure
```text
mobile-app-engagement-retention-analysis/
├── README.md
├── mobile_app_engagement_retention_analysis.ipynb
└── requirements.txt
```

## Note
All user-level data and experimental outcomes are synthetic and were generated for educational and portfolio purposes.
