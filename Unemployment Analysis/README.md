#  Unemployment Analysis with Python

A comprehensive data analysis project investigating unemployment trends in India, with a special focus on the **impact of COVID-19** on unemployment rates. This project follows the end-to-end machine learning workflow — from data collection and cleaning to model training, evaluation, and deployment.

---

##  Project Structure

```
Unemployment Analysis with Python/
│
├── csv files/
│   ├── Unemployment in India.csv              # Primary dataset (May 2019 – Jun 2020)
│   └── Unemployment_Rate_upto_11_2020.csv     # Secondary dataset (Jan 2020 – Oct 2020)
│
├── Unemployment_Analysis.ipynb                # Main Jupyter Notebook
├── requirements.txt                           # Python dependencies
└── README.md                                  # Project documentation
```

---

##  Objectives

1. **Analyze unemployment rate data** representing unemployed people as a percentage of the labour force.
2. **Use Python** for data cleaning, exploration, and visualization of unemployment trends.
3. **Investigate the impact of COVID-19** on unemployment rates across Indian states.
4. **Identify key patterns** or seasonal trends in the data.
5. **Present insights** that could inform economic or social policies.

---

##  Workflow

| Step | Description |
|------|-------------|
| 1. Define the Problem | Understand the objective (regression problem — predicting unemployment rates) |
| 2. Collect & Prepare Data | Load datasets, handle missing values, preprocess features |
| 3. Exploratory Data Analysis | Visualize distributions, correlations, and regional/temporal trends |
| 4. Feature Engineering | Extract date features, encode categoricals, select relevant features |
| 5. Split the Data | Train/test split (80/20) |
| 6. Choose a Model | Random Forest Regressor |
| 7. Train the Model | Fit model on training data |
| 8. Evaluate the Model | RMSE, MAE, R² Score |
| 9. Improve the Model | Hyperparameter tuning |
| 10. Deploy (Optional) | Prediction function for new inputs |

---

##  Datasets

### Dataset 1: `Unemployment in India.csv`
- **Period**: May 2019 – June 2020
- **Records**: 768 rows × 7 columns
- **Coverage**: 28 Indian states and UTs — Rural & Urban breakdown

### Dataset 2: `Unemployment_Rate_upto_11_2020.csv`
- **Period**: January 2020 – October 2020
- **Records**: 267 rows × 9 columns
- **Coverage**: 28 states — includes geographic coordinates

### Key Columns
| Column | Description |
|--------|-------------|
| `Region` | Indian state or UT |
| `Date` | Month-end date |
| `Estimated Unemployment Rate (%)` | Target variable |
| `Estimated Employed` | Number of employed persons |
| `Estimated Labour Participation Rate (%)` | Active workforce percentage |
| `Area` | Rural / Urban |

---

##  Installation & Setup


. Install Dependencies

```bash
pip install -r requirements.txt
```

 Launch Jupyter Notebook

```bash
jupyter notebook Unemployment_Analysis.ipynb
```

---

##  Key Insights

- **COVID-19 Impact**: Unemployment rates surged dramatically from ~7% to over **23%** during April–May 2020 (national lockdown period).
- **Urban vs Rural**: Urban areas saw higher and more volatile unemployment rates compared to rural regions.
- **State-wise Variation**: States like **Tripura, Haryana, and Jharkhand** showed the highest unemployment peaks during the pandemic.
- **Recovery Trend**: Post-lockdown (June–October 2020), unemployment rates gradually recovered but remained elevated above pre-COVID levels.
- **Labour Participation**: A strong negative correlation exists between labour participation rate and unemployment rate.

---

##  Machine Learning Model

- **Algorithm**: Random Forest Regressor
- **Features Used**: Month, Year, Area (Rural/Urban), Estimated Employed, Labour Participation Rate, Region (encoded)
- **Evaluation Metrics**: RMSE, MAE, R² Score
- **Hyperparameter Tuning**: GridSearchCV with cross-validation

---

##  Libraries Used

| Library | Purpose |
|---------|---------|
| `pandas` | Data manipulation and analysis |
| `numpy` | Numerical computations |
| `matplotlib` | Static visualizations |
| `seaborn` | Statistical visualizations |
| `plotly` | Interactive visualizations |
| `scikit-learn` | Machine learning model |
| `scipy` | Statistical testing |
| `statsmodels` | Time series analysis |

---


##  Author

ANUJ YADAV
 
 
##  License

This project is for educational and analytical purposes as part of an AI internship program.

