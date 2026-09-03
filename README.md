# Predictive Maintenance — ML & Data Analysis
## Dataset

- **Source:** [AI4I 2020 Predictive Maintenance Dataset (Kaggle)](https://www.kaggle.com/datasets/stephanmatzka/predictive-maintenance-dataset-ai4i-2020)
- **Size:** 10,000 rows, 14 columns
- **Target:** `Machine failure` (0 = no failure, 1 = failure)
```
| Column | Meaning |
|---|---|
| `Type` | Product quality variant: L (50%), M (30%), H (20%) |
| `Air temperature [K]` | Ambient temperature |
| `Process temperature [K]` | Process temperature |
| `Rotational speed [rpm]` | Spindle speed |
| `Torque [Nm]` | Applied torque |
| `Tool wear [min]` | Accumulated tool wear |
| `Machine failure` | **Target** — did the machine fail? |
| `TWF, HDF, PWF, OSF, RNF` | Specific failure modes (tool wear, heat, power, overstrain, random) |
```

## Project structure

```
predictive-maintenance-ml-data-analysis/
├── data/
│   ├── raw/            # original dataset (ai4i2020.csv)
│   └── processed/      # cleaned data after understanding step
├── notebooks/
│   ├── 01_data_understanding.ipynb            # inspect columns, check quality, clean
│   ├── 02_exploratory_data_analysis.ipynb     # plots & patterns in the data
│   ├── 03_linear_logistic_regression.ipynb    # first models
│   └── 04_forest_regression.ipynb             # random forest
├── requirements.txt
└── README.md
```

## Tech stack

- **Python 3.12.9**
- **pandas / polars** — data handling
- **scikit-learn** — models & metrics
- **matplotlib / seaborn / plotly** — visualization
- **Jupyter** — notebooks

## References

Tutorials and docs used to help:

- [Random Forest classifier (DataCamp)](https://www.datacamp.com/tutorial/random-forests-classifier-python)
- [Random Forest regression (DataCamp)](https://www.datacamp.com/tutorial/random-forest-regression)
- [Linear regression with scikit-learn (DataCamp)](https://www.datacamp.com/tutorial/sklearn-linear-regression)
- [Understanding logistic regression (DataCamp)](https://www.datacamp.com/tutorial/understanding-logistic-regression-python)
- [StatQuest (YouTube) for fundaments as r², p-value, linear and logistic regression, random forest regression](https://www.youtube.com/@statquest)
- [scikit-learn docs](https://scikit-learn.org/stable/) ·
  [pandas](https://pandas.pydata.org/) ·
  [polars](https://pola.rs/) ·
  [matplotlib](https://matplotlib.org/) ·
  [plotly](https://plotly.com/python/)

