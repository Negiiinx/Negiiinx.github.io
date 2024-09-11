---
title: "A Machine Learning-Based Prediction of Hospital Mortality in Mechanically Ventilated ICU Patients"
collection: publications
category: manuscripts
permalink: /publication/2024-09-09-ml-prediction-hospital-mortality
date: 2024-09-09
venue: "PLOS ONE"
paperurl: 'https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0309383'
---

Background
Mechanical ventilation (MV) is vital for critically ill ICU patients but carries significant mortality risks. This study aims to develop a predictive model to estimate hospital mortality among MV patients, utilizing comprehensive health data to assist ICU physicians with early-stage alerts.

Methods
We developed a Machine Learning (ML) framework to predict hospital mortality in ICU patients receiving MV. Using the MIMIC-III database, we identified 25,202 eligible patients through ICD-9 codes. We employed backward elimination and the Lasso method, selecting 32 features based on clinical insights and literature. Data preprocessing included eliminating columns with over 90% missing data and using mean imputation for the remaining missing values. To address class imbalance, we used the Synthetic Minority Over-sampling Technique (SMOTE). We evaluated several ML models, including CatBoost, XGBoost, Decision Tree, Random Forest, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), and Logistic Regression, using a 70/30 train-test split. The CatBoost model was chosen for its superior performance in terms of accuracy, precision, recall, F1-score, AUROC metrics, and calibration plots.

Results
The study involved a cohort of 25,202 patients on MV. The CatBoost model attained an AUROC of 0.862, an increase from an initial AUROC of 0.821, which was the best reported in the literature. It also demonstrated an accuracy of 0.789, an F1-score of 0.747, and better calibration, outperforming other models. These improvements are due to systematic feature selection and the robust gradient boosting architecture of CatBoost.

Conclusion
The preprocessing methodology significantly reduced the number of relevant features, simplifying computational processes, and identified critical features previously overlooked. Integrating these features and tuning the parameters, our model demonstrated strong generalization to unseen data. This highlights the potential of ML as a crucial tool in ICUs, enhancing resource allocation and providing more personalized interventions for MV patients.
