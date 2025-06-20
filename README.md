# 🚢 Titanic Survival Prediction

> Can we predict who survived the Titanic disaster?  
> This project uses machine learning to classify survival outcomes based on passenger characteristics from the Titanic dataset.

---

## 📖 Background

The sinking of the RMS Titanic in 1912 remains one of the most infamous maritime disasters.  
Using passenger data provided by Kaggle, this project explores patterns in survival and builds predictive models to estimate the likelihood of survival based on features like age, gender, class, and family size.

---

## 💾 Dataset Overview

The dataset includes two main CSV files:

- `train.csv`: 891 labeled records used for training  
- `test.csv`: 418 unlabeled records used for prediction  
- `gender_submission.csv`: Baseline submission for scoring

### Key Features
| Feature | Description |
|---------|-------------|
| `Pclass` | Ticket class (1st, 2nd, 3rd) |
| `Sex` | Gender |
| `Age` | Age in years |
| `SibSp` | # of siblings/spouses aboard |
| `Parch` | # of parents/children aboard |
| `Fare` | Ticket fare |
| `Embarked` | Port of Embarkation (C/Q/S) |
| `Survived` | Target: 1 = survived, 0 = did not survive |

---

## 🎯 Objective

1. Perform exploratory data analysis to understand key drivers of survival  
2. Engineer useful features such as family size and travel alone flags  
3. Build and compare classification models to predict survival  
4. Generate a Kaggle submission using the best-performing model

---

## 🛠️ Tools Used

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-00599C?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0D76A8?style=for-the-badge&logo=python&logoColor=white)

---

## 🔍 Approach

| Step | Description |
|------|-------------|
| 🧹 Data Cleaning | Handled missing values in `Age` and `Embarked`; dropped `Cabin` |
| 🛠 Feature Engineering | Created `FamilySize`, `IsAlone`, and binned `Age` |
| 📊 EDA | Visualized survival by gender, age, class, and family composition |
| ⚙️ Modeling | Trained Logistic Regression, Random Forest, and XGBoost |
| 📈 Evaluation | Compared test set performance using accuracy and confusion matrix |
| 📤 Submission | Created `.csv` file for Kaggle leaderboard submission |

---

## 🧪 Model Evaluation

| Model | Test Accuracy |
|-------|---------------|
| Logistic Regression | ~0.79 |
| Random Forest | ~0.83 |
| **XGBoost** *(Best)* | **~0.85** ✅

> XGBoost performed best in terms of accuracy and robustness.

---

