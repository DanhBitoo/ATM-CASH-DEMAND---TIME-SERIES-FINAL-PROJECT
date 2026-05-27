# ATM Cash Demand Forecasting (NN5 Competition Dataset)

A research and development project for forecasting cash withdrawal demand across a network of 111 ATMs, utilizing the standard **NN5 Time Series Forecasting Competition** dataset. This project implements a hybrid approach, combining traditional statistical models (ARIMA, SARIMAX) with modern machine learning techniques (Global LightGBM), structured according to professional MLOps standards.

---

## 📁 Repository Structure

The repository is organized following Data Science best practices to ensure a clear separation between data, experimental source code, and reporting outputs:

```text
NN5-Project/
│
├── data/                  # Project data management (Ignored by Git)
│   ├── raw/               # Original dataset (NN_COMPLETE.xls)
│   └── processed/         # Cleaned data and engineered features (.pkl format)
│
├── notebooks/             # Jupyter Notebooks for analysis and modeling
│   ├── 01_data_preprocess.ipynb  # Data loading, EDA, and robust Feature Engineering
│   └── 02_model_training.ipynb   # Stationarity testing, Model Training & Evaluation
│
├── reports/               # Output artifacts for analytical reporting
│   ├── NN5_report.pdf     # Detailed project analysis report (PDF)
│   └── figures/           # Auto-generated plots (EDA, SHAP, Actual vs Predicted)
│
├── models/                # Stored weights of trained models (.pkl, .txt, etc.)
│
├── .gitignore             # Files/folders excluded from version control (data/, models/)
├── README.md              # Project documentation and setup guide (This file)
└── requirements.txt       # Python dependencies and exact version requirements