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
| `Victim Sex` | Sex of the victim |
| `Victim Age` | Age of the victim |
| `Victim Race` | Race of the victim |
| `Victim Ethnicity` | Ethnic background of the victim |
| `Victim Count` | Number of victims involved in the incident |
| `Perpetrator Sex` | Sex of the perpetrator |
| `Perpetrator Age` | Age of the perpetrator |
| `Perpetrator Race` | Race of the perpetrator |
| `Perpetrator Ethnicity` | Ethnic background of the perpetrator |
| `Perpetrator Count` | Number of perpetrators involved |
| `Relationship` | Relationship between victim and perpetrator |
| `Weapon` | Weapon used during the incident |



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

## 📈 Key Findings from Crime Data Analysis

This document summarizes the key findings derived from the exploratory data analysis and time series analysis of the US Crime Dataset.

## 1. Univariate Analysis

-   **Crime Type:** 'Murder or Manslaughter' dominates the dataset, accounting for approximately 98.6% of all recorded incidents. 'Manslaughter by Negligence' constitutes a minor 1.4%.
-   **Crime Solved Status:** A significant majority of crimes (69.8%) are reported as 'Solved', while 30.2% remain 'Unsolved'.
-   **Victim and Perpetrator Sex Distribution:** Both victims and perpetrators are predominantly male. Males represent about 75.1% of victims and 74.7% of perpetrators. Females account for 24.9% of victims and 21.0% of perpetrators. The sex of perpetrators is 'Unknown' in 4.3% of cases.
-   **Race and Ethnicity:** 'White' individuals are the most frequently recorded race for both victims (46.8%) and perpetrators (42.4%). For ethnicity, 'Unknown' is the largest category for both victims (68.1%) and perpetrators (69.9%), followed by 'Not Hispanic'.
-   **Relationship between Victim and Perpetrator:** The relationship between the victim and perpetrator is 'Unknown' in 43.2% of cases, followed by 'Acquaintance' (19.9%) and 'Stranger' (15.3%).
-   **Weapon Used:** 'Handgun' is by far the most common weapon, used in 49.7% of incidents. 'Knife' (14.9%) and 'Blunt Object' (10.5%) are the next most frequent.
-   **Age Distribution:** Victim ages are broadly distributed, with the 21-30 age group showing the highest percentage (33.1%). Perpetrator ages are concentrated in the 21-30 age group (37.3%), followed by 31-40 (20.9%).

## 2. Bivariate Analysis

-   **Top Agencies by Crime Count:** The `Chicago Municipal Police` recorded the highest number of incidents, followed by `Houston Municipal Police` and `Detroit Municipal Police`.
-   **Crime Type vs. Solved Status:** 'Manslaughter by Negligence' has an exceptionally high solved rate (95.7%). 'Murder or Manslaughter' cases are solved approximately 69.8% of the time.
-   **Sex Interaction Pattern:** Male perpetrators are involved in a high proportion of crimes against both male (75.1%) and female (24.9%) victims. Female perpetrators primarily victimize males (77.5%).
-   **Race and Ethnicity Interaction:** The analysis reveals a strong tendency for crimes to occur within the same racial groups, particularly for Black and White individuals. Similarly, 'Not Hispanic' perpetrators primarily victimize 'Not Hispanic' individuals.
-   **Victim Age vs. Perpetrator Age:** A hexbin plot indicates a strong correlation between victim and perpetrator ages, suggesting that individuals often commit crimes against those in similar age brackets.
-   **Crime Solved by Agency Type:** 'State Police' (82.3%) and 'Tribal Police' (92.6%) demonstrate the highest crime-solved rates. 'County Police' and 'Municipal Police' show solved rates of approximately 67-68%.

## 3. Spatial Mapping

-   **Geographical Distribution of Crimes:** California, Texas, and Florida consistently appear as the states with the highest overall crime incidents, victim counts, and perpetrator counts, highlighting them as major crime hotspots.
-   **Unsolved Crimes by State:** California leads in the number of unsolved crimes, followed by New York and Texas.

## 4. Time Series Analysis

-   **Overall Crime Trends (1980-2014):** The total number of annual crime incidents generally shows a decreasing trend over the analyzed period, as confirmed by the 3-year rolling mean.
-   **Autocorrelation:** Significant autocorrelation was observed in the overall incident data, as well as for specific categories like 'Murder or Manslaughter', 'Solved/Unsolved Crimes', 'Victim Count', and 'Perpetrator Count'. This suggests that past crime rates influence future rates, indicating potential for time series forecasting.
-   **Seasonal Patterns:** A monthly incident heatmap revealed distinct seasonal patterns, with certain months consistently showing higher or lower crime counts across different years.
-   **Trends in Specific Crime Types:** 'Murder or Manslaughter' incidents align with the overall decreasing trend. 'Manslaughter by Negligence' remains low and relatively stable.
-   **Solved vs. Unsolved Trends:** Both solved and unsolved crime counts generally follow the overall decreasing trend, with solved crimes consistently outnumbering unsolved cases annually.


## 🛠 Tools & Libraries
- **Python 3**
- `pandas` – data manipulation  
- `numpy` – numerical computation  
- `matplotlib` & `seaborn` – visualization  
- `statsmodels` – time series analysis  
- `plotly` – interactive visualizations  
