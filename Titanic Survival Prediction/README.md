#  Titanic Survival Prediction

A complete end-to-end machine learning project that predicts whether a passenger aboard the RMS Titanic survived or not, built using the classic Titanic dataset.

---

##  Project Overview

The sinking of the Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, the RMS Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This project builds a classification model to predict survival based on passenger attributes.

**Problem Type:** Binary Classification  
**Target Variable:** `Survived` (0 = Did not survive, 1 = Survived)

---

##  Project Structure

```
TITANIC SURVIVAL PREDICTION/
│
├── Titanic-Dataset.csv          # Raw dataset
├── titanic_survival.ipynb       # Main Jupyter Notebook
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

---

##  Dataset Description

The dataset contains **892 rows** and **12 columns**:

| Column      | Description                                      |
|-------------|--------------------------------------------------|
| PassengerId | Unique identifier for each passenger             |
| Survived    | Survival (0 = No, 1 = Yes) — **Target variable** |
| Pclass      | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)        |
| Name        | Full name of the passenger                       |
| Sex         | Gender of the passenger                          |
| Age         | Age in years                                     |
| SibSp       | Number of siblings/spouses aboard                |
| Parch       | Number of parents/children aboard                |
| Ticket      | Ticket number                                    |
| Fare        | Passenger fare                                   |
| Cabin       | Cabin number                                     |
| Embarked    | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

##  Project Workflow

The notebook follows the standard ML pipeline:

1. **Define the Problem** — Binary classification: predict survival
2. **Data Collection & Preparation** — Load CSV, inspect data types, handle missing values
3. **Exploratory Data Analysis (EDA)** — Visualize distributions, correlations, survival rates
4. **Feature Engineering** — Extract titles, create family size, bin ages/fares
5. **Split the Data** — 80% training / 20% testing with stratification
6. **Model Selection** — Compare Logistic Regression, Random Forest, and XGBoost
7. **Model Training** — Train all three models on the training set
8. **Model Evaluation** — Accuracy, Precision, Recall, F1-Score, Confusion Matrix, ROC-AUC
9. **Model Improvement** — GridSearchCV hyperparameter tuning
10. **Final Results & Insights** — Feature importance, final performance summary

---

##  Setup & Installation

### Prerequisites
- Python 3.9 or higher
- pip package manager

### Step 1: Clone / Navigate to the Project Directory

```bash
cd "TITANIC SURVIVAL PREDICTION"
```

### Step 2: (Optional) Create a Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate        # On Windows
source venv/bin/activate     # On macOS/Linux
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook titanic_survival.ipynb
```

---

##  Models Used

| Model                | Description                                     |
|----------------------|-------------------------------------------------|
| Logistic Regression  | Baseline linear model for binary classification |
| Random Forest        | Ensemble of decision trees, robust to overfitting |
| XGBoost              | Gradient boosting — typically the best performer |

---

##  Key Insights

- **Gender** is the strongest predictor — females had a significantly higher survival rate
- **Passenger Class** matters — 1st class passengers survived at a higher rate
- **Age** — children had a higher survival probability (women & children first)
- **Fare** — higher fares correlated with better survival odds
- **Family Size** — solo travelers and very large families had lower survival rates

---

##  Technologies Used

| Library       | Version  | Purpose                           |
|---------------|----------|-----------------------------------|
| pandas        | 2.2.2    | Data manipulation and analysis    |
| numpy         | 1.26.4   | Numerical computing               |
| matplotlib    | 3.8.4    | Data visualization                |
| seaborn       | 0.13.2   | Statistical data visualization    |
| scikit-learn  | 1.4.2    | Machine learning algorithms       |
| xgboost       | 2.0.3    | Gradient boosting classifier      |
| jupyter       | 1.0.0    | Interactive notebook environment  |

---

##  Results Summary

The best-performing model achieves:
- **Accuracy:** ~84%
- **ROC-AUC Score:** ~0.88

---

##  Author

ANUJ YADAV

---

## 📄 License

This project is for educational purposes.
