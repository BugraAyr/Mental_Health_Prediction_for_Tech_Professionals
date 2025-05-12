#  Mental Health Disorder Prediction in the Tech Industry

This project uses machine learning to predict whether a person currently has a mental health disorder based on the 2016 "Mental Health in Tech" survey conducted by OSMI.

##  Dataset

- **Title:** Mental Health in Tech - 2016 Survey  
- **Source:** [Kaggle - Mental Health in Tech 2016](https://www.kaggle.com/datasets/osmi/mental-health-in-tech-2016)  
- **Description:** Contains responses from over 1,400 participants working in the tech industry, focusing on mental health awareness, treatment, and workplace support.

##  Objective

To build a predictive model that can accurately determine whether an individual currently experiences a mental health disorder using workplace, personal, and demographic factors.

##  Features and Target

- **Target Variable:** `currently_have_mental_health_disorder`
- **Feature Engineering:**
  - Dropped irrelevant variables (`age`, `year`, etc.)
  - One-hot encoding for categorical variables
  - Spearman correlation used for feature inspection

##  Machine Learning Models

Several models were trained and evaluated. Below are the results sorted by accuracy:

| Model                  | Accuracy (%) |
|------------------------|--------------|
| Random Forest        | **88.89**     |
| AdaBoost               | 88.61        |
| Gradient Boosting      | 88.33        |
| XGBoost                | 87.50        |
| Logistic Regression    | 83.89        |
| K-Nearest Neighbors    | 82.78        |
| Decision Tree          | 82.78        |

##  Evaluation

- **Metrics Used:**
  - Accuracy
  - Classification Report (Precision, Recall, F1-Score)
  - Confusion Matrix
  - ROC AUC Score

- **Best Performing Model:** Random Forest  
- Full evaluation and visualizations are available in the `notebooks` folder.

##  Correlation Analysis

Spearman correlation was used to explore the relationship between features. Features with |r| > 0.5 were visualized in a heatmap to detect strong relationships and possible multicollinearity.

