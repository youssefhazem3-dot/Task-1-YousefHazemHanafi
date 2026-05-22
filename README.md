# Titanic Survival Prediction - DecodeLabs Internship Project 1

## 📌 Project Overview

This is my first project as a **DecodeLabs Intern**.  
The project focuses on analyzing the Titanic dataset and building a basic Machine Learning model to predict whether a passenger survived or not based on passenger information such as age, gender, ticket class, fare, and family-related features.

The main goal of this project is to practice the complete beginner-friendly Machine Learning workflow, starting from data loading and understanding, then data cleaning and visualization, and finally training and evaluating a predictive model.

---

## 🎯 Project Objectives

- Load and understand the Titanic dataset.
- Explore the structure, data types, missing values, and general statistics of the data.
- Clean and preprocess the dataset to make it suitable for analysis and modeling.
- Perform exploratory data analysis to understand survival patterns.
- Visualize numerical and categorical features.
- Build a baseline Machine Learning model using Logistic Regression.
- Evaluate the model using a confusion matrix and classification report.

---

## 🗂️ Dataset

The dataset used in this project is the Titanic dataset.

It contains passenger information such as:

- Passenger ID
- Survival status
- Passenger class
- Name
- Gender
- Age
- Number of siblings/spouses aboard
- Number of parents/children aboard
- Ticket number
- Fare
- Cabin
- Embarkation port

### Target Variable

| Column | Description |
|---|---|
| `Survived` | Indicates whether the passenger survived or not. `0 = Not Survived`, `1 = Survived` |

### Dataset Shape

- Rows: `891`
- Columns: `12`

---

## 🧹 Data Cleaning & Preprocessing

The preprocessing stage included:

- Removing unnecessary columns such as:
  - `PassengerId`
  - `Name`
  - `Ticket`
  - `Cabin`
- Handling missing values.
- Filling missing `Age` values using the median age.
- Dropping rows with missing values where needed.
- Converting selected columns to suitable data types.
- Checking and removing duplicated records.
- Preparing the dataset for model training.

---

## 📊 Exploratory Data Analysis

The analysis stage included:

- Checking numerical and categorical columns.
- Detecting outliers using box plots.
- Studying feature distributions using histograms and KDE plots.
- Visualizing categorical features using count plots.
- Creating a heatmap to compare survival patterns.
- Using pair plots to observe relationships between features.

### Key Observations

- The dataset contains missing values, especially in the `Cabin` and `Age` columns.
- Survival rate is not equally distributed between passengers.
- Gender and passenger class appear to have a strong relationship with survival.
- First-class passengers generally had a higher survival rate than third-class passengers.
- Female passengers had a much higher survival rate than male passengers.

---

## 🤖 Machine Learning Model

A baseline classification model was built using:

- **Logistic Regression**

### Model Workflow

1. Define features and target variable.
2. Split the dataset into training and testing sets.
3. Train the Logistic Regression model.
4. Predict survival results on the test set.
5. Evaluate the model using:
   - Confusion Matrix
   - Precision
   - Recall
   - F1-score
   - Accuracy

---

## 📈 Model Evaluation

The baseline model achieved an accuracy of approximately:

```text
Accuracy: 56%
```

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|---|---:|---:|---:|---:|
| 0 - Not Survived | 0.56 | 0.99 | 0.71 | 85 |
| 1 - Survived | 0.67 | 0.03 | 0.06 | 69 |

| Metric | Score |
|---|---:|
| Accuracy | 0.56 |
| Macro Avg F1-Score | 0.38 |
| Weighted Avg F1-Score | 0.42 |

> Note: This model is a first baseline model. The recall for survived passengers is low, so future improvements can focus on better preprocessing, feature engineering, and trying stronger classification models.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📁 Project Structure

```text
.
├── DecodeLabs_Project1.ipynb
├── titanic.csv
└── README.md
```

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repository-name.git
```

### 2. Navigate to the project folder

```bash
cd your-repository-name
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Open the notebook

```bash
jupyter notebook DecodeLabs_Project1.ipynb
```

### 5. Run all cells

Make sure that the `titanic.csv` file is in the same folder as the notebook before running the project.

---

## 🚀 Future Improvements

Possible improvements for the next version:

- Apply better categorical encoding techniques.
- Use feature scaling where needed.
- Create new features such as family size or title extracted from passenger names.
- Try other models such as:
  - Decision Tree
  - Random Forest
  - Gradient Boosting
  - Support Vector Machine
- Use cross-validation for better evaluation.
- Improve recall for survived passengers.
- Build a cleaner Machine Learning pipeline using Scikit-learn.

---

## ✅ Conclusion

This project helped me practice the basic Machine Learning workflow using a real-world dataset.  
It includes data understanding, preprocessing, visualization, model training, and evaluation.

As my first DecodeLabs internship project, it represents the starting point of my hands-on journey in data analysis and Machine Learning.

---

## 👨‍💻 Author

**Yousef Hazem**  
Computer Engineering Student  
AI & Machine Learning Enthusiast  
DecodeLabs Intern
