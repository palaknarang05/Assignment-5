# Employee Attrition Prediction using Decision Tree and Random Forest Classification

## Student Information

**Name:** Palak Narang  
**Registration Number:** 23BCE11819  
**Application Number:** IN26011657  
**Batch Number:** 1A  
**Program:** AI/ML Internship Program  
**Department:** Computer Science and Engineering  
**University:** VIT Bhopal University

---

## Objective

The objective of this project is to develop **Decision Tree** and **Random Forest** classification models to predict employee attrition based on demographic, professional, and work-related attributes. The project also compares the performance of both models using standard evaluation metrics and feature importance analysis to determine the more effective classifier.

---

## Dataset

**Dataset:** IBM HR Analytics Employee Attrition & Performance Dataset

**Source:** Kaggle

https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

---

## Libraries Used

The project was implemented in Python using the following libraries:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Methodology

### 1. Data Loading
- Loaded the IBM HR Analytics Employee Attrition dataset using Pandas.
- Displayed the first five records for initial inspection.

### 2. Data Understanding
- Identified numerical and categorical features.
- Examined the dataset using `shape()`, `info()`, and `describe()`.
- Identified **Attrition** as the target variable.

### 3. Data Preprocessing
- Checked for missing values.
- Removed unnecessary columns if present.
- Encoded categorical variables using Label Encoding.
- Split the dataset into **80% training** and **20% testing** sets.

### 4. Model Development

Two machine learning models were developed:

#### Model 1
- Decision Tree Classifier

#### Model 2
- Random Forest Classifier (`n_estimators = 100`)

Both models were trained using the same training dataset and used to predict employee attrition on the testing dataset.

### 5. Model Evaluation

The models were evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score

Additional analyses included:

- Confusion Matrix for Decision Tree
- Confusion Matrix for Random Forest
- Random Forest Feature Importance Plot

---

## Results

### Decision Tree Classifier
- Good classification performance
- Simple and interpretable model
- More susceptible to overfitting

### Random Forest Classifier
- Higher Accuracy and F1-Score
- Better generalization on unseen data
- More robust due to ensemble learning

Important features influencing employee attrition included:

- Monthly Income
- OverTime
- Age
- Total Working Years
- Years At Company

---

## Model Comparison

| Metric | Decision Tree | Random Forest |
|---------|--------------|---------------|
| Accuracy | Higher than baseline | Generally Higher |
| Precision | Good | Better |
| Recall | Good | Better |
| F1-Score | Good | Better |

The Random Forest model consistently outperformed the Decision Tree model by reducing overfitting and producing more stable predictions.

---

## Conclusion

This project successfully developed Decision Tree and Random Forest classification models to predict employee attrition. Both models demonstrated good predictive performance after preprocessing and encoding the dataset. However, the Random Forest classifier generally achieved better Accuracy, Precision, Recall, and F1-score due to its ensemble learning approach, which combines multiple decision trees to reduce variance and improve generalization. Feature importance analysis revealed that variables such as Monthly Income, OverTime, Age, Total Working Years, and Years At Company significantly influence employee attrition. A limitation of Decision Trees is their tendency to overfit complex datasets, while Random Forest models require greater computational resources and are less interpretable. Overall, Random Forest proved to be the more reliable model for predicting employee attrition.

---

## Bonus Challenge

A simple hyperparameter tuning experiment was performed by increasing the number of estimators in the Random Forest model from **100** to **200**.

**Observation:**
Increasing the number of trees slightly improved model stability while increasing training time. The performance improvement was minimal, indicating that 100 estimators were sufficient for this dataset.

---

## Repository Structure

```text
MPONLINE-Assignment-5/
│
├── Assignment-5.ipynb
├── README.md
└── .gitignore
```

---

## Author

**Palak Narang**

B.Tech Computer Science and Engineering  
VIT Bhopal University
