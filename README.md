# Mental Health Data Kaggle Competition Season 4 Episode 11

## For full project view please visit **Dags Hub** https://dagshub.com/maimunul/Mental-Health-Data-Competition-s4-e11-Kaggle
---------

# 🧠 Welcome to the *Exploring Mental Health Data* Notebook!

Welcome to our Kaggle competition project **Exploring Mental Health Data!** In this project, we aim to explore, analyze, and model data from a synthetic mental health survey to identify factors associated with depression. This competition is part of Kaggle's **2024 Playground Series**, designed to challenge and enhance our machine learning skills. Let’s dive in and uncover insights from the data!


# 🏆 Kaggle Notebook: Mental Health Analysis and Prediction 🧠

## 📋 Table of Contents
1. **📦 Libraries and Setup**  
   * Importing all the required libraries and setting up the environment.
2. **🛠️ Data Loading and Initial Analysis**  
   * Loading the training and test datasets.  
   * Performing basic checks for missing and duplicate values.
3. **🔧 Preprocessing Pipeline**  
   * Custom transformers and pipeline construction for feature engineering and cleaning.
4. **🚂 Model Training with Stratified Cross-Validation**  
   * Training models with **stratified cross-validation** for reliable evaluation.
5. **🎯 Best Model Selection and Performance**  
   * Identifying the best model based on cross-validation accuracy.  
   * Evaluating the model on the training dataset.
6. **📤 Saving Predictions**  
   * Exporting predictions for the best model and all other models.  
   * Saving results to CSV files.
7. **📊 Predicted Probability Visualization**  
   * Visualizing the distribution of predicted probabilities for the test set.
8. **🎉 Conclusions and Next Steps**  
   * Summarizing key findings and outlining potential improvements.


---

## 🎯 Introduction

### Competition Goal 🏁
The goal of this competition is to explore mental health survey data and identify key factors associated with depression. By analyzing various features, we aim to make predictions that can accurately indicate the presence of depression.

### Key Deliverables 📋
We will produce predictions for each entry in the test set, aiming to achieve high accuracy in identifying individuals who may experience depression.

### Evaluation Metric 🎯
Submissions are evaluated using the **Accuracy Score**, meaning our predictions will be judged based on the proportion of correct classifications.

### Approach Outline 🧩
Our approach to the competition will include the following steps:
1. **Data Exploration and Visualization**: Gain initial insights into the dataset.
2. **Feature Engineering**: Create and select meaningful features.
3. **Model Training and Tuning**: Build, evaluate, and tune models.
4. **Submission Preparation**: Prepare final predictions for submission.

![Project Banner](https://github.com/maimunul/Mental-Health-Data-Kaggle-Competition-S4-E11/blob/main/Screenshot%202025-03-26%20163422.png)


# 📊 Dataset Overview: Understanding Depression Risk Factors among Adults

### 📝 Dataset Context
>  The following table describes each feature in the dataset and its relevance.

---

### 📌 **Feature Descriptions**

| **Feature**                                               | **Description**                                                                                     |
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| **👤 Name**                                               | Participant's name.                                                                                 |
| **🚻 Gender**                                             | Participant's gender (Male/Female).                                                                 |
| **🎂 Age**                                                | Participant's age (18-60).                                                                          |
| **🏙️ City**                                               | Participant's city of residence.                                                                    |
| **👔 Working Professional or Student**                    | Indicates whether the participant is a working professional or a student.                           |
| **💼 Profession**                                         | Participant's current profession.                                                                   |
| **📚 Academic Pressure**                                  | Level of academic workload, rated on a scale from 1 to 5.                                           |
| **📈 Work Pressure**                                      | Level of work-related workload, rated on a scale from 1 to 5.                                       |
| **🎓 CGPA**                                               | Cumulative Grade Point Average.                                                                     |
| **📖 Study Satisfaction**                                 | Satisfaction level with studies, rated on a scale from 1 to 5.                                      |
| **💼 Job Satisfaction**                                   | Satisfaction level with job, rated on a scale from 1 to 5.                                          |
| **🛏️ Sleep Duration**                                    | Average hours of sleep per night.                                                                   |
| **🍲 Dietary Habits**                                     | Information about participant’s eating habits.                                                      |
| **🎓 Degree**                                             | Highest degree or qualification obtained by the participant.                                        |
| **🧠 Have you ever had suicidal thoughts?**               | Indicates if the participant has had suicidal thoughts (Yes/No).                                    |
| **⏰ Work/Study Hours**                                   | Average daily hours spent on work or study.                                                         |
| **💵 Financial Stress**                                   | Level of financial stress, rated on a scale from 1 to 5.                                            |
| **👪 Family History of Mental Illness**                   | Indicates if there is a family history of mental illness (Yes/No).                                  |
| **🩺 Depression**                                         | Represents whether the participant is at risk of depression (Yes/No), based on lifestyle and demographic factors. |

---

Each feature is essential for understanding various lifestyle and environmental factors that may influence depression risk. The dataset could be used in predictive modeling, trend analysis, and further research on mental health and wellness interventions.
