# Titanic Survival Prediction Project

---

## Introduction

This project aims to predict the survival of passengers aboard the Titanic using machine learning techniques. The dataset contains various features such as passenger class, age, gender, and ticket fare, among others.

---

## Data Exploration

### Number of Null Values in Each Column
![image](https://github.com/17-doha/Titanic-Survival-Prediction-Project/assets/65771031/afe66ac6-5ec4-4b07-adf8-a3865cf39c88)


### Survival Rate by Passenger Class
![image](https://github.com/17-doha/Titanic-Survival-Prediction-Project/assets/65771031/c72270a7-9977-4e6d-a7fa-5316f7b48242)


### Survival Rate by Gender
![image](https://github.com/17-doha/Titanic-Survival-Prediction-Project/assets/65771031/e0a5db69-d999-4602-8993-b4d753d01387)


### Age Distribution of Survivors vs Non-Survivors
![image](https://github.com/17-doha/Titanic-Survival-Prediction-Project/assets/65771031/496b17c1-8254-46af-b5ad-2a5d219702e8)


### Correlation Matrix of Numeric Columns
![image](https://github.com/17-doha/Titanic-Survival-Prediction-Project/assets/65771031/ae4ac584-484b-4903-ae92-9e9b74532b51)


---

## Data Cleaning

1. **Extracted some information from the cabin and dropped it:** Utilized the 'Cabin' feature to derive the 'Deck' information, filling any missing values with 'Unknown', and subsequently dropping the 'Cabin' column.
2. **Grouped ages into categories and labeled them:** Created age groups based on predefined bins and labeled them accordingly. Any missing values were labeled as 'Unknown'.
3. **Filled missing values in the Embarked column:** Used the mode of the 'Embarked' column to fill in the two missing values.
4. **Removed outliers from numeric columns:** Employed the z-score method to identify and remove outliers from numeric columns, specifically focusing on features like 'Fare' and 'FamilySize'.

---

## Feature Engineering and Selection

- Converted categorical variables into one-hot encoded format.
- Encoded ordinal variables using label encoding.
- Scaled numerical features using MinMaxScaler.
- Engineered new feature 'FamilySize' from SibSp and Parch.
- Dropped irrelevant features such as PassengerId, Ticket, Name, SibSp, and Parch.

---

## Machine Learning Models

### Model Evaluation

- **Support Vector Machines (SVM):** Achieved an accuracy of 84.34%.
- **K-Nearest Neighbors (KNN):** Achieved an accuracy of 81.93%.
- **Categorical Naive Bayes:** Achieved the highest accuracy of 80.12%.
- **Decision Tree:** Achieved an accuracy of 80.12%.
- **Neural Networks:** Achieved an accuracy of 79.51%.
- **Random Forest:** Achieved an accuracy of 78.92%.
- **Multinomial Naive Bayes:** Achieved an accuracy of 76.51%.
- **Gaussian Naive Bayes:** Achieved an accuracy of 72.89%.

Each model was evaluated using accuracy, precision, recall, and F1-score metrics, as well as cross-validation to assess generalization performance.


---

## Conclusion

Categorical Naive Bayes and Support Vector Machine models performed the best, achieving accuracies of 0.8012 and 0.8434, respectively. Further optimization and ensemble techniques could potentially improve the performance of the models.

---

## Author

Doha Hemdan Ismail

## Date

19/5/2024
