# 🚢 Titanic Survival Prediction | Machine Learning Project

<img width="640" height="480" alt="WhatsApp Image 2026-06-19 at 6 20 05 PM" src="https://github.com/user-attachments/assets/f43290a5-3d90-4d59-8ecf-f7949f66ec09" />


<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/f58b2270-0124-4f03-9f2f-8ed91fc87e28" />


<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/572cfc5b-8805-43b8-8edf-859054f57fd8" />

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📖 Project Overview

This project focuses on predicting passenger survival aboard the Titanic using Machine Learning techniques in Python.

The analysis includes data cleaning, exploratory data analysis (EDA), feature engineering, visualization, model training, and evaluation. The goal is to identify the key factors that influenced survival and build a predictive classification model.

---

## 🎯 Business Objective

The objective is to analyze historical passenger data and develop a model capable of predicting whether a passenger survived based on demographic and travel-related characteristics.

This project demonstrates an end-to-end Data Analytics and Machine Learning workflow commonly used in real-world business environments.

---

## 📂 Dataset

Source:

- Titanic Dataset (Kaggle)

Features include:

| Variable | Description |
|-----------|------------|
| PassengerId | Unique passenger identifier |
| Survived | Target variable (0 = No, 1 = Yes) |
| Pclass | Passenger class |
| Name | Passenger name |
| Sex | Gender |
| Age | Passenger age |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Ticket | Ticket number |
| Fare | Ticket fare |
| Cabin | Cabin number |
| Embarked | Port of embarkation |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- VS Code
- Git & GitHub

---

## 🔍 Exploratory Data Analysis (EDA)

The following analyses were performed:

### Survival Distribution

- Overall survival rate
- Survivor vs non-survivor comparison

### Gender Analysis

- Survival rate by gender
- Male vs female comparison

### Age Analysis

- Age distribution
- Relationship between age and survival

### Passenger Class Analysis

- Survival by ticket class
- Socioeconomic impact on survival

### Missing Values Analysis

- Identification of null values
- Missing data treatment strategy

---

## 📊 Key Insights

### Women had significantly higher survival rates.

### First-class passengers survived more frequently than third-class passengers.

### Younger passengers generally had a higher probability of survival.

### Ticket fare showed a positive relationship with survival probability.

### Socioeconomic status played an important role in passenger outcomes.

---

## 🧹 Data Cleaning

The following preprocessing steps were applied:

### Missing Values

python
df["Age"] = df["Age"].fillna(df["Age"].median())
df["Embarked"] = df["Embarked"].fillna(df["Embarked"].mode()[0])


### Categorical Encoding

python
df["Sex"] = df["Sex"].map({"male": 0, "female": 1})

df["Embarked"] = df["Embarked"].map({
    "S": 0,
    "C": 1,
    "Q": 2
})


---

## 🤖 Machine Learning Model

### Algorithm Used

python
RandomForestClassifier()


### Features Selected

python
[
    "Pclass",
    "Sex",
    "Age",
    "Fare",
    "Embarked"
]


### Target Variable

python
Survived


---

## 📈 Model Evaluation

Evaluation Metric:

python
Accuracy Score


Model Performance:

text
Accuracy: XX.XX%


Replace the value above with your final result.

---

## 📉 Feature Importance Analysis

The project also evaluates the importance of each feature used by the Random Forest model.

Typical influential variables include:

1. Sex
2. Fare
3. Age
4. Pclass
5. Embarked

---

## 📁 Project Structure

text
Titanic-Survival-Prediction
│
├── train.csv
├── test.csv
├── titanic_analysis.py
├── README.md
│
├── images
│   ├── survival_distribution.png
│   ├── gender_survival.png
│   ├── age_distribution.png
│   └── feature_importance.png
│
└── requirements.txt


---

## 🚀 Installation

Clone the repository:

bash
git clone https://github.com/yourusername/titanic-survival-prediction.git


Move into the project folder:

bash
cd titanic-survival-prediction


Install dependencies:

bash
pip install pandas numpy matplotlib seaborn scikit-learn


---

## ▶️ Run the Project

bash
python titanic_analysis.py


---

## 💡 Skills Demonstrated

✔️ Data Cleaning

✔️ Exploratory Data Analysis (EDA)

✔️ Data Visualization

✔️ Feature Engineering

✔️ Machine Learning

✔️ Classification Models

✔️ Model Evaluation

✔️ Python Programming

✔️ GitHub Portfolio Development

---

## 📚 What I Learned

Throughout this project I strengthened my skills in:

- Data preparation and preprocessing
- Exploratory Data Analysis
- Business-oriented insights generation
- Machine Learning fundamentals
- Model evaluation techniques
- Professional project documentation

---

## 🔮 Future Improvements

- Hyperparameter tuning
- Cross-validation
- Additional feature engineering
- Comparison with other algorithms
- Deployment using Streamlit

---

## 👨‍💻 Author

### Pedro Pérez

*Data Analyst | Python | SQL | Power BI | Machine Learning*

Passionate about transforming data into actionable insights and building data-driven solutions that support business decision-making.
