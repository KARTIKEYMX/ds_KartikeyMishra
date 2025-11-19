
---

# Web3 Trading Team — Data Science Assignment

**Candidate:** Kartikey Mishra  
**Repository Name:** ds_KartikeyMishra  

---

## 📂 Folder Structure

ds_KartikeyMishra/  
├── notebook_1.ipynb        → Data loading, cleaning, EDA, merge, sentiment summary, insights  
├── notebook_2.ipynb        → Predictive modeling (ARIMA, Random Forest), comparison, conclusion  
├── csv_files/              → Raw datasets (historical_data.csv, fear_greed_index.csv)  
├── outputs/                → Saved charts, plots, and merged_dataset.csv  
├── ds_report.pdf           → Final summarized report  
└── README.md               → Instructions and notes  

---

## 🚀 How to Run

1. Open the notebooks in Google Colab.  
2. Mount Google Drive and set the root directory (`ds_KartikeyMishra`).  
3. Run `notebook_1.ipynb` first to generate merged dataset and EDA outputs.  
4. Run `notebook_2.ipynb` for feature engineering, ARIMA, Random Forest, and model comparison.  
5. All plots and outputs are saved automatically in the `outputs/` folder.  

---

## 📊 Datasets

- Historical Trader Data (Hyperliquid) → `historical_data.csv`  
- Bitcoin Market Sentiment (Fear & Greed Index) → `fear_greed_index.csv`  

Columns were standardized and renamed for consistency:  
- `value` → `fg_value`  
- `classification` → `fg_class`  

---

## 🎯 Objective

Analyze how trading behavior (profitability, risk, volume, leverage) aligns or diverges from overall market sentiment (Fear vs Greed).  
Identify hidden trends or signals that could influence smarter trading strategies.  

---

## 🔎 Key Insights

- Fear days → largest trade sizes and highest profits.  
- Extreme Greed days → moderate trade sizes but lower profitability.  
- Neutral days → lowest activity and smallest PnL.  
- Predictive models (ARIMA, Random Forest) struggled due to small dataset size, highlighting the need for more historical data.  

---

## 📈 Models Applied

- ARIMA (time series forecasting)  
  - RMSE ≈ 490M  
  - Struggled due to very few observations.  

- Random Forest Regression (machine learning)  
  - RMSE ≈ 5.1M  
  - R² ≈ -7.5 (worse than baseline).  

---

## 📌 Next Steps

1. Collect larger datasets (hundreds of daily records).  
2. Re‑train ARIMA with proper frequency information (daily time series).  
3. Include leverage and side (long/short) analysis.  
4. Explore advanced models (XGBoost, LSTM) once more data is available.  

---

## 📝 Submission Notes

- All work was done in Google Colab.  
- Outputs (plots, merged dataset) are stored in `outputs/`.  
- Final report (`ds_report.pdf`) summarizes insights with figures.  
- GitHub repository mirrors the exact structure for compliance.  

---

## 🔗 Colab Links

- Open notebook_1 in Colab: https://colab.research.google.com/drive/1CmsHcU1d0lJmc8qrNSZblYHZ4YREEQQK?usp=sharing
- Open notebook_2 in Colab: https://colab.research.google.com/drive/1GBuTBZb5Tl7CHKzPSx0UWU5DaFRfv7tZ?usp=sharing 
