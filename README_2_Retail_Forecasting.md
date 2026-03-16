# UK Retail Sales Forecasting (ONS Data)
### Python · ARIMA · Prophet · Power BI · Time-Series Forecasting

> **Business problem:** UK retailers need reliable sales forecasts to plan stock, staffing, and marketing spend. This project analyses 10MB+ of official ONS retail sales data to uncover trends, build forecasting models, and deliver a strategic outlook through 2026.

---

## Results at a glance

| Metric | Value |
|---|---|
| Forecast accuracy improvement | ~15–20% vs baseline |
| Forecast horizon | Through 2026 |
| Data source | UK Office for National Statistics (ONS) — official government retail index |
| Models used | ARIMA, Facebook Prophet |
| Deliverable | Interactive Power BI dashboard with trend and forecast visuals |

---

## Project architecture

```
ONS UK Retail Sales Index (10MB+ raw data)
        ↓
  Data cleaning & EDA (Python — Pandas, Matplotlib, Seaborn)
        ↓
  Time-series modelling (ARIMA + Prophet)
        ↓
  Forecast through 2026
        ↓
  Power BI dashboard — trends, seasonality, strategic insights
```

---

## Step-by-step process

### Notebook 1 — Data cleaning & EDA
- Loaded and inspected ONS retail sales dataset (10MB+)
- Checked for null values, handled missing data, standardised date formats
- Exploratory analysis: sales trends by category, seasonal patterns, year-on-year growth
- Visualised post-pandemic recovery trajectory across retail sectors

### Notebook 2 — Forecasting models
- Applied **ARIMA** model — tuned p, d, q parameters via AIC minimisation
- Applied **Facebook Prophet** — captured seasonality, holiday effects, and trend changepoints
- Compared model performance; Prophet outperformed ARIMA on long-horizon forecasts
- Achieved **15–20% improvement** in forecast accuracy vs naive baseline
- Generated forecasts through 2026 for strategic planning use

### Power BI dashboard
- Interactive dashboard presenting historical trends and 2026 forecast
- Breakdown by retail category: food, clothing, household goods, online
- Designed for non-technical stakeholders — clear visual storytelling

---

## Key findings

- **Strong seasonal peaks** around the holiday season (Nov–Dec) across all categories
- **Post-pandemic recovery** is clearly visible in online retail — sustained above pre-2020 levels
- **Household goods** show long-term growth opportunity through 2026
- **Clothing retail** remains volatile — higher forecast uncertainty band

---

## Tech stack

| Tool | Purpose |
|---|---|
| Python (Pandas, Matplotlib, Seaborn) | Data cleaning, EDA, visualisation |
| Statsmodels | ARIMA model |
| Facebook Prophet | Seasonal time-series forecasting |
| Power BI | Interactive dashboard and business insights |
| GitHub | Version control |

---

## Files in this repo

| File | Description |
|---|---|
| `retail-store-project.ipynb` | Notebook 1 — data cleaning, EDA, exploratory visualisations |
| `grocery-sales-store-file2.ipynb` | Notebook 2 — ARIMA and Prophet forecasting models |
| `README.md` | Project overview |

---

## How to run

1. Clone the repo
2. Install dependencies:
```
pip install pandas matplotlib seaborn statsmodels prophet
```
3. Run `retail-store-project.ipynb` first (EDA and cleaning)
4. Then run `grocery-sales-store-file2.ipynb` (forecasting models)

---

*Project associated with MSc Data Analytics — De Montfort University (2025)*
