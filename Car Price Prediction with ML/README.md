#  Car Price Prediction with Machine Learning

A complete end-to-end machine learning project that predicts the **selling price of used cars** based on features like brand, year, present price, fuel type, transmission, and more.

---

##  Problem Statement

Predicting the resale value of a used car is a classic **regression problem**. Given a set of car attributes, the goal is to build a model that accurately estimates the selling price — helping buyers and sellers make informed decisions.

---

##  Project Structure

```
Car Price Prediction with Machine Learning/
│
├── car data.csv                        # Raw dataset
├── Car_Price_Prediction.ipynb          # Main Jupyter Notebook
├── requirements.txt                    # Python dependencies
└── README.md                           # Project documentation
```

---

##  Dataset Description

The dataset (`car data.csv`) contains **301 records** of used cars with the following features:

| Column          | Description                                      |
|-----------------|--------------------------------------------------|
| `Car_Name`      | Name/Model of the car                            |
| `Year`          | Year of purchase                                 |
| `Selling_Price` | Price at which the car is being sold (target)    |
| `Present_Price` | Current ex-showroom price of the car             |
| `Driven_kms`    | Total kilometers driven                          |
| `Fuel_Type`     | Type of fuel (Petrol / Diesel / CNG)             |
| `Selling_type`  | Dealer or Individual                             |
| `Transmission`  | Manual or Automatic                              |
| `Owner`         | Number of previous owners                        |

---

##  Machine Learning Workflow

1. **Define the Problem** — Regression task: Predict `Selling_Price`
2. **Collect & Prepare Data** — Load CSV, handle missing values, encode categoricals
3. **Exploratory Data Analysis (EDA)** — Visualize distributions, correlations, and outliers
4. **Feature Engineering** — Create `Car_Age` from `Year`, encode categorical features
5. **Split the Data** — 80% Training / 20% Testing
6. **Choose a Model** — Random Forest Regressor (+ Linear Regression as baseline)
7. **Train the Model** — Fit on training data
8. **Evaluate the Model** — MAE, MSE, RMSE, R² Score
9. **Improve the Model** — Hyperparameter tuning with GridSearchCV

---

##  Tech Stack

| Tool            | Purpose                              |
|-----------------|--------------------------------------|
| **Python 3.10+**| Programming Language                 |
| **Pandas**      | Data manipulation and preprocessing  |
| **NumPy**       | Numerical computations               |
| **Matplotlib**  | Data visualization                   |
| **Seaborn**     | Statistical visualizations           |
| **Scikit-learn**| Machine learning models & evaluation |
| **Jupyter**     | Interactive notebook environment     |

---

##  Getting Started


### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Launch Jupyter Notebook

```bash
jupyter notebook Car_Price_Prediction.ipynb
```

### 3. Run All Cells

Go to **Kernel → Restart & Run All** to execute the full pipeline.

---

##  Model Performance

| Metric              | Linear Regression | Random Forest |
|---------------------|:-----------------:|:-------------:|
| **MAE**             | ~1.8              | ~0.7          |
| **RMSE**            | ~3.0              | ~1.2          |
| **R² Score**        | ~0.82             | ~0.96         |

> *Results may vary slightly based on train/test split randomness.*

---

##  Key Visualizations in the Notebook

- Distribution of Selling Price (Histogram)
- Correlation Heatmap
- Fuel Type & Transmission vs Selling Price (Box Plots)
- Actual vs Predicted Price Scatter Plot
- Feature Importance Bar Chart

---

##  Real-World Applications

- **Online Car Marketplaces** (OLX, CarDekho, Cars24) — Suggest fair pricing
- **Insurance Companies** — Estimate vehicle value for coverage
- **Bank Loan Assessment** — Evaluate collateral value for auto loans
- **Fleet Management** — Optimize resale timing for company vehicles

---

##  Author

ANUJ YADAV

---

##  License

This project is for educational purposes. Dataset is publicly available on [Kaggle]
