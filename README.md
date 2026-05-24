# 🌊 Global Weather Trend Forecasting
## PM Accelerator — Data Science Technical Assessment

**By: Yeabsira Yirgu**

---

## 🚀 About PM Accelerator
PM Accelerator is a world-class product management training program that equips
aspiring and experienced PMs with real-world skills through hands-on projects,
mentorship from industry leaders, and a powerful professional network —
accelerating careers at top tech companies globally.

---

## 📊 Project Overview
Advanced data science analysis of the Global Weather Repository dataset
(32,264 records, 41 features) to forecast future weather trends using
multiple machine learning models.

---

## ✅ What Was Completed

### Data Cleaning & Preprocessing
- Handled missing values and dropped null rows
- Replaced -9999 anomalous values in air quality columns with median
- Removed impossible outliers in wind speed and temperature
- Normalized key features using MinMaxScaler

### Advanced EDA
- Temperature and precipitation distributions
- Global correlation heatmap
- Time series analysis of weather trends
- Anomaly detection using Isolation Forest (5% contamination)

### Forecasting Models
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- Ensemble Model (average of all 3)
- Evaluated using MAE, RMSE, and R² metrics
- 30-day future temperature forecast with confidence intervals

### Unique Analyses
- **Climate Analysis** — Monthly patterns, seasonal variations, climate zones
- **Environmental Impact** — Air quality correlation with weather parameters
- **Feature Importance** — Random Forest and Gradient Boosting importance scores
- **Spatial Analysis** — Interactive global temperature and air quality maps
- **Geographical Patterns** — Weather differences across continents

---

## 📁 Project Structure
\`\`\`
weather-analysis-repo/
├── analysis.ipynb                    ← Main Jupyter notebook
├── GlobalWeatherRepository.csv       ← Dataset
├── requirements.txt                  ← Python dependencies
├── README.md                         ← This file
├── eda_temperature_precipitation.png
├── correlation_matrix.png
├── anomaly_detection.png
├── time_series.png
├── model_comparison.png
├── feature_importance.png
├── climate_analysis.png
├── environmental_impact.png
├── geographical_patterns.png
├── forecast_30days.png
├── project_summary.png
├── spatial_temperature.html
└── spatial_airquality.html
\`\`\`

---

## 🛠️ How to Run

### Option 1 — Google Colab (Recommended)
1. Upload `analysis.ipynb` to Google Colab
2. Upload `GlobalWeatherRepository.csv` to the Colab files panel
3. Run all cells in order

### Option 2 — Local
1. Clone the repo:
\`\`\`bash
git clone https://github.com/Yeabsira96/weather-analysis.git
cd weather-analysis
\`\`\`
2. Install dependencies:
\`\`\`bash
pip install -r requirements.txt
\`\`\`
3. Launch Jupyter:
\`\`\`bash
jupyter notebook analysis.ipynb
\`\`\`

---

## 📦 Dataset
- **Source:** [Global Weather Repository — Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository/code)
- **Records:** 32,264
- **Features:** 41
- **Coverage:** Countries worldwide
- **Date Range:** May 2024 — October 2024

---

## 🤖 Model Results Summary


============================================================
Model                          MAE     RMSE       R²
============================================================
Linear Regression            0.395    0.507    0.115
Random Forest                1.766    1.848  -10.755
Gradient Boosting            1.761    1.841  -10.666
Ensemble                     1.179    1.275   -4.595
============================================================

*(Fill in your actual results from Cell 9 output)*

---

## 🔮 Key Findings
- Global average temperature: ~25.5°C
- Tropical zones are significantly warmer than polar regions
- Humidity and feels-like temperature are most correlated with actual temperature
- Anomaly detection flagged high-altitude cities like Addis Ababa as outliers
- Air quality is worst in densely populated Asian and African cities

---

*Built with Python | pandas | scikit-learn | matplotlib | seaborn | plotly*
