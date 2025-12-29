# 📊 Crime Time Series Analysis (1980–2014)

## 📌 Project Overview
This project presents an exploratory and time series analysis of crime incident data spanning **1980 to 2014**.  
The objective is to uncover long-term trends, seasonal patterns, persistence, and volatility in crime incidents using statistical and visualization techniques.

The analysis applies concepts from **rolling statistics, time series decomposition, autocorrelation (ACF/PACF), and trend analysis**, providing insights useful for policy analysis, forecasting, and data-driven decision-making.

---

## 🎯 Objectives
- Analyze long-term crime trends over time  
- Identify seasonal and cyclical patterns  
- Examine temporal persistence using autocorrelation analysis  
- Assess volatility and structural changes  
- Prepare the data for time series forecasting models  

---

## 🗂 Dataset Description
The dataset contains recorded crime incidents with the following relevant features:

| Column | Description |
|------|------------|
| `Year` | Year of incident (1980–2014) |
| `Month` | Month of incident (1–12) |
| `Agency Name` | Reporting law enforcement agency |
| `Agency Type` | Type of agency |
| `Crime Type` | Category of crime |
| `Crime Solved` | Whether the crime was solved |
| `Victim Count` | Number of victims |
| `Perpetrator Count` | Number of perpetrators |


## 🧠 Methods & Techniques Used

### 1️⃣ Exploratory Data Analysis (EDA)
- Incident aggregation by year and month  
- Decade-wise comparisons  
- Distribution analysis of victims and perpetrators  

### 2️⃣ Trend Analysis
- Rolling mean smoothing  
- Visualization of long-term crime behavior  

### 3️⃣ Seasonality Analysis
- Monthly aggregation across years  
- Detection of recurring seasonal patterns  

### 4️⃣ Volatility Analysis
- Rolling standard deviation  
- Identification of unstable periods  

### 5️⃣ Time Series Decomposition
- Additive decomposition into:
  - Trend
  - Seasonal
  - Residual components  

### 6️⃣ Autocorrelation Analysis
- Autocorrelation Function (ACF)  
- Partial Autocorrelation Function (PACF)  
- Evaluation of persistence and model suitability  

---

## 📈 Key Findings
- Crime incidents exhibit a **strong long-term trend**, rather than random behavior  
- Significant **temporal dependence**, confirmed by slow ACF decay  
- Evidence of **non-stationarity**, requiring differencing for forecasting  
- Certain periods show **higher volatility**, indicating structural changes  
- Monthly data suggests potential **seasonal crime patterns**  

---

## 🛠 Tools & Libraries
- **Python 3**
- `pandas` – data manipulation  
- `numpy` – numerical computation  
- `matplotlib` & `seaborn` – visualization  
- `statsmodels` – time series analysis  
- `plotly` – interactive visualizations  

---

## 📂 Project Structure
```text
crime-time-series-analysis/
│
├── data/
│   └── crime_data.csv
│
├── notebooks/
│   └── crime_analysis.ipynb
│
├── figures/
│   └── plots/
│
├── README.md
└── requirements.txt
