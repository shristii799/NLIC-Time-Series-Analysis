# NLIC Time Series Analysis

A machine learning project focused on time series analysis of Nepal Life Insurance Company (NLIC), combining statistical methods, signal processing, and deep learning to investigate trends, seasonality, stationarity, and forecasting performance.

## Overview

This project explores historical NLIC data using a range of time series analysis techniques and forecasting models. It examines underlying trends, moving averages, seasonal patterns, and statistical properties before applying traditional statistical models and deep learning approaches.

The project also implements custom linear regression and compares forecasting performance using Root Mean Squared Error (RMSE).

## Key Features

- **Trend Detection:** Identify long-term trends in the time series.
- **LOESS Smoothing:** Smooth noisy observations to reveal underlying patterns.
- **Mann–Kendall Test:** Assess the presence and direction of monotonic trends.
- **Moving Average and Detrending:** Analyze smoothed trends and separate trend components from the original series.
- **Seasonality Analysis:** Investigate recurring temporal patterns.
- **ACF and PACF Analysis:** Examine autocorrelation and partial autocorrelation to understand temporal dependencies.
- **Fourier Transform:** Analyze frequency components and periodic patterns.
- **Stationarity Testing:** Evaluate the statistical properties of the time series.
- **Deep Learning:** Implement LSTM and GRU models to learn sequential patterns.
- **Custom Linear Regression:** Develop a regression-based forecasting approach.
- **Statistical Forecasting:** Apply ARIMA and SARIMA models.
- **Model Evaluation:** Compare forecasting performance using RMSE.

## Methodology

The project follows a structured time series analysis workflow:

1. **Data Preparation:** Load and inspect the dataset, prepare the time series, and perform necessary preprocessing.
2. **Exploratory Analysis:** Visualize the data and investigate its overall behavior.
3. **Trend Analysis:** Apply LOESS smoothing, moving averages, the Mann–Kendall test, and detrending methods.
4. **Seasonality and Dependence:** Analyze recurring patterns using seasonality analysis, ACF, PACF, and Fourier transforms.
5. **Stationarity Analysis:** Perform statistical tests to assess stationarity.
6. **Model Development:** Implement custom linear regression, ARIMA, SARIMA, LSTM, and GRU forecasting models.
7. **Model Evaluation:** Compare model predictions using RMSE.

## Models and Techniques

| Category                  | Methods                                          |
| ------------------------- | ------------------------------------------------ |
| Trend analysis            | LOESS, Mann–Kendall, moving averages, detrending |
| Seasonality and frequency | Seasonality analysis, Fourier transform          |
| Temporal dependence       | ACF, PACF                                        |
| Statistical testing       | Stationarity tests                               |
| Regression                | Custom linear regression                         |
| Statistical forecasting   | ARIMA, SARIMA                                    |
| Deep learning             | LSTM, GRU                                        |
| Evaluation                | RMSE comparison                                  |

## Technologies Used

- **Python**
- **Google Colab**
- **Pandas** and **NumPy**
- **Matplotlib** and **Seaborn**, where used
- **Statsmodels** for statistical time series analysis, where used
- **Scikit-learn** for relevant machine learning utilities, where used
- **TensorFlow/Keras** or another deep learning framework, depending on the implementation

## Repository Structure

```text
NLIC-Time-Series-Analysis/
├── NLIC_Time_Series_Analysis.ipynb
├── data/
│   └── nlic.csv
└── README.md
```

- `NLIC_Time_Series_Analysis.ipynb` contains the analysis, visualizations, model implementations, and evaluation.
- `data/` contains the CSV dataset used by the notebook.
- `README.md` documents the project and its methodology.



## Model Evaluation

Forecasting models are evaluated using **Root Mean Squared Error (RMSE)** to compare the magnitude of prediction errors.

RMSE is calculated as:

[
RMSE = \sqrt{\frac{1}{n}\sum\_{i=1}^{n}(y_i-\hat{y}\_i)^2}
]

where:

- (y_i) represents the actual observation.
- (\hat{y}\_i) represents the predicted observation.
- (n) is the number of observations.

Lower RMSE indicates smaller prediction errors on the evaluated dataset. Comparisons should use the same test period and forecasting setup to be meaningful.

## Results

The notebook contains the analysis and model evaluation. Quantitative findings, plots, and the best-performing model can be documented here after reviewing the actual results.
