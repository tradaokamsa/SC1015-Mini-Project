# SC1015 Mini Project: Students' Performance Analysis

## Introduction
This project focuses on analyzing students' performance using data from a learning management system (LMS). By leveraging machine learning algorithms, we aim to predict students' academic performance levels, which are crucial for implementing targeted educational strategies.

## Problem Definition
Using the educational dataset collected from the learning management system (LMS), we aim to develop a machine learning model that predicts the academic performance levels of students based on their demographic, academic background, and behavioral features. The performance levels are categorized as Fail, Satisfied, Good, Very Good and Excellent, corresponding to specific grade/mark intervals.

## Motivation
The motivation behind predicting student academic performance levels lies in the desire to improve educational outcomes and support student success. By accurately identifying factors that contribute to student performance, educational institutions can implement targeted interventions and support systems to enhance learning experiences and outcomes for students.

## Dataset
The dataset used in this project is sourced from the UCI Machine Learning Repository and is accessible [here](https://archive.ics.uci.edu/dataset/320/student+performance).

## Brief Process Walkthrough (In Order)
1. **Data Cleaning and Preprocessing**:
   - Handling missing values, duplicates, and outliers.
   - Creating a new feature 'Total' to summarize students' grades across different terms.

2. **Exploratory Data Analysis (EDA)**:
   - Analysis of categorical and numerical variables to understand their influence on the 'Total' performance score.

3. **Model Training Attempts**:
   - **Attempt 1 (Baseline Models):**
     - Initial models were trained using only demographic and behavioral data.
     - **Decision Tree Classifier**: Average accuracy: 0.72
     - **SVM Classifier**: Average accuracy: 0.43
     - **KNN Classifier**: Average accuracy: 0.48
     - **Logistic Regression Classifier**: Average accuracy: 0.45
     - **Random Forest Classifier**: Average accuracy: 0.73
     - **Gradient Boosting Classifier**: Average accuracy: 0.59
   
   - **Attempt 2 (Enhanced Models with Historical Grades):**
     - Incorporated G1 and G2 grades as additional features to enhance model predictions.
     - **Decision Tree Classifier**: Average accuracy: 0.89
     - **SVM Classifier**: Average accuracy: 0.76
     - **KNN Classifier**: Average accuracy: 0.77
     - **Logistic Regression Classifier**: Average accuracy: 0.77
     - **Random Forest Classifier**: Average accuracy: 0.89
     - **Gradient Boosting Classifier**: Average accuracy: 0.87

4. **Results Analysis**:
   - Enhanced models with G1 and G2 grades demonstrated superior predictive abilities, confirming the hypothesis that past academic performance is indicative of future outcomes.
   - The significant improvement in accuracy across all models highlights the importance of including historical academic data for robust performance prediction.


## Results, Conclusion and Discussion
Our exploration into predicting students' academic performance revealed several key insights:
- Initially, models that only utilized demographic and behavioral data provided a baseline for performance prediction. However, these models alone were not highly predictive of the students' final grades.
- The inclusion of past performance data (G1 and G2 grades) significantly enhanced the accuracy of our predictive models. This suggests that students' earlier performance is a critical indicator of their final outcomes, emphasizing the importance of continuous assessment.
- We observed a remarkable improvement across all models when incorporating historical grades (G1 and G2). The Random Forest Classifier and Decision Tree Classifier stood out, both reaching an impressive accuracy of 0.89 in the enhanced setup, showing their capacity to effectively utilize the additional data. The Gradient Boosting Classifier also performed well, with an accuracy increase to 0.87, underscoring its robustness and suitability for handling the nuanced patterns in educational data. Other models such as the SVM, KNN, and Logistic Regression also showed notable improvements, highlighting the importance of comprehensive feature inclusion for predictive accuracy in educational settings.
- The study underscores the utility of more complex models that can capture nonlinear relationships and interactions between features when predicting student performance.
- Based on these findings, educational institutions should consider implementing systems that regularly monitor and analyze students' performance throughout the academic year. This continuous assessment can provide valuable early warnings and insights, enabling targeted interventions to support students who may be at risk of underperforming.

These conclusions highlight the potential of machine learning in educational settings, demonstrating its capability to provide actionable insights that can lead to improved educational strategies and student outcomes.

## Lessons Learned
Throughout this project, we have gained insights into:
- The critical role of data preprocessing and feature engineering in enhancing model performance.
- Learning how to use different and new machine learning models, such as Random Forest Classifier, KNN Classifier,... to predict variables.
- The strengths and limitations of various machine learning algorithms in handling educational data.

## Contributors
- Hoang Phong
- Dao Hai Nam
- Syed Abu Thahir
