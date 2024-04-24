# SC1015 Mini Project: Students' Performance Analysis

## Introduction
This project focuses on analyzing students' performance using data from a learning management system (LMS). By leveraging machine learning algorithms, we aim to predict students' academic performance levels, which are crucial for implementing targeted educational strategies.

## Problem Definition
Using the educational dataset collected from the learning management system (LMS), we aim to develop a machine learning model that predicts the academic performance levels of students based on their demographic, academic background, and behavioral features. The performance levels are categorized as Fail, Satisfied, Good, Very Good and Excellent, corresponding to specific grade/mark intervals.

## Motivation
The motivation behind predicting student academic performance levels lies in the desire to improve educational outcomes and support student success. By accurately identifying factors that contribute to student performance, educational institutions can implement targeted interventions and support systems to enhance learning experiences and outcomes for students.

## Dataset
The dataset used in this project is sourced from the UCI Machine Learning Repository and is accessible [here](https://archive.ics.uci.edu/dataset/320/student+performance).

## Models Used
- Random Forest Classifier
- Decision Tree Classifier
- Gradient Boosting Classifier
- KNN Classifier
- SVM Classifier
- Logistic Regression Classifier

## Brief Process Walkthrough (In Order)
1. **Data Cleaning and Preprocessing**:
   - Handling missing values, duplicates, and outliers.
   - Creating a new feature 'Total' to summarize students' grades across different terms.

2. **Exploratory Data Analysis (EDA)**:
   - Analysis of categorical and numerical variables to understand their influence on the 'Total' performance score.

3. **Model Training Attempts**:
   - **Attempt 1 (Baseline Models):**
     - Initial models were trained using only demographic and behavioral data, including: 'age', 'school', 'address', 'Medu', 'Fedu', 'studytime', 'failures', 'higher', 'freetime', 'goout', 'health', 'Dalc', 'Walc' and 'absences'.
     - **Random Forest Classifier**: Average accuracy: 0.69
     - **Decision Tree Classifier**: Average accuracy: 0.67
     - **Gradient Boosting Classifier**: Average accuracy: 0.53
     - **KNN Classifier**: Average accuracy: 0.45
     - **SVM Classifier**: Average accuracy: 0.41
     - **Logistic Regression Classifier**: Average accuracy: 0.41
   
   - **Attempt 2 (Enhanced Models with Historical Grades):**
     - Incorporated G1 and G2 grades as additional features to enhance model predictions.
     - **Random Forest Classifier**: Average accuracy: 0.88
     - **Decision Tree Classifier**: Average accuracy: 0.86
     - **Gradient Boosting Classifier**: Average accuracy: 0.83
     - **SVM Classifier**: Average accuracy: 0.76
     - **Logistic Regression Classifier**: Average accuracy: 0.75
     - **KNN Classifier**: Average accuracy: 0.72

4. **Results Analysis**:
   - Enhanced models with G1 and G2 grades demonstrated superior predictive abilities, confirming the hypothesis that past academic performance is indicative of future outcomes.
   - The significant improvement in accuracy across all models highlights the importance of including historical academic data for robust performance prediction.


## Results, Conclusion and Discussion
Our exploration into predicting students' academic performance revealed several key insights:
- Initially, models that only utilized demographic and behavioral data provided a baseline for performance prediction. However, these models alone were not highly predictive of the students' final grades.
- The inclusion of past performance data (G1 and G2 grades) significantly enhanced the accuracy of our predictive models. This suggests that students' earlier performance is a critical indicator of their final outcomes, emphasizing the importance of continuous assessment.
- We observed a remarkable improvement across all models when incorporating historical grades (G1 and G2). The Random Forest Classifier stood out, leading with an impressive accuracy of around 0.88 in the enhanced setup, showing its capacity to effectively utilize the additional data. The Decision Tree Classifier also performed well, with an accuracy increase to 0.86, underscoring its robustness and suitability for handling the nuanced patterns in educational data. Other models such as the SVM, KNN, Gradient Boosting and Logistic Regression also showed notable improvements, highlighting the importance of comprehensive feature inclusion for predictive accuracy in educational settings.
- The study underscores the utility of more complex models that can capture nonlinear relationships and interactions between features when predicting student performance.
- Based on these findings, educational institutions should consider implementing systems that regularly monitor and analyze students' performance throughout the academic year. This continuous assessment can provide valuable early warnings and insights, enabling targeted interventions to support students who may be at risk of underperforming.
- The model not only showed the effect of past test results on the final score which is quite obvious but also the importance of health, free time and going out. This shows that educational institutions should be mindful of the physical as well as mental health of the students. Students should be given enough breaks and schools maybe can arrange a retreat with the students to improve their mental health. This will not only improve the wellbeing of the student but also their final grades. 

These conclusions highlight the potential of machine learning in educational settings, demonstrating its capability to provide actionable insights that can lead to improved educational strategies and student outcomes.

## Lessons Learned
Throughout this project, we have gained insights into:
- The critical role of data preprocessing and feature engineering in enhancing model performance.
- Learning how to use different and new machine learning models, such as Random Forest Classifier, KNN Classifier,... to predict variables.
- The strengths and limitations of various machine learning algorithms in handling educational data.

## Contributors
- Hoang Phong ()
- Dao Hai Nam ()
- Syed Abu Thahir ()

## References
- [Random Forest Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [Decision Tree Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
- [Gradient Boosting Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html)
- [KNN Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
- [SVM Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)
- [Logistic Regression Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
- https://archive.ics.uci.edu/dataset/320/student+performance


