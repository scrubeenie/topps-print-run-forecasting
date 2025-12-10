# 🧮 Topps Print Run Forecasting  
### *(NBA Project – MLB expansion planned)*

Machine learning project analyzing and forecasting **Topps Now print runs** using:

- Feature engineering  
- Exploratory data analysis  
- Random Forest regression  
- Log-transformed modeling for skewed distributions  
- Visualizations (matplotlib, seaborn)  
- Future Power BI dashboards  

This project builds a predictive framework for understanding how factors such as rookies, superstars, multi-player cards, team tier, and rare inserts influence daily sports card print runs.

---

## 📌 Project Question  
**Can we predict print runs using publicly available card data?  
Which card attributes most strongly influence demand?**

---

## 📊 Current Model Performance

The current model uses a **Random Forest Regressor** with engineered features.

**Model Results (Log scale):**

- **R² Score:** 0.587  
- **Log MAE:** 0.741  
- **Log RMSE:** 0.983  

➡️ *This means the model explains ~59% of the variance in print runs — strong given the small dataset and high volatility of Topps Now print behavior.*

---

## 🧱 Feature Engineering

The model includes custom engineered features:

- **IsRookie** – flags rookie cards  
- **IsVet** – flags veteran players  
- **SPInserts** – identifies rare short-print insert cards  
- **HasAutoRelic** – identifies autograph/relic cards  
- **IsSuperstar** – derived from superstar list (Curry, Jokic, Wembanyama, etc.)  
- **TeamTier** – teams categorized into market tiers  
- **IsMultiPlayer** – single vs multi-player card indicator  

These features significantly improved model stability and predictive power.

---

## 🔍 Exploratory Data Analysis Highlights

- Superstar and rookie cards show significantly higher median print runs  
- High-tier market teams (Lakers, Celtics, Warriors) exhibit stronger demand   
- Distribution of print runs is heavily skewed → *log transformation required*  
- Multi-player cards behave differently than single-player cards  

---

## 🤖 Modeling Approach

1. Cleaned and normalized Print Run values  
2. Created engineered features  
3. Applied log transformation to target variable  
4. Split data: 80% training / 20% testing  
5. Trained Random Forest Regressor (n=300)  
6. Evaluated MAE, RMSE, and R²  
7. Visualized predictions vs actual values  
8. Analyzed feature importances  

---

## 📈 Next Steps

- Expand dataset to include MLB Topps Now cards  
- Merge historical players' popularity metrics  
- Build **Power BI dashboards** for interactive analysis   
- Test alternative models: GradientBoosting, XGBoost, LightGBM  
- Add external features such as:
  - Player performance data  
  - Milestone moments
  - Google player trends

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| **Topps_Now_NBA.ipynb** | Full analysis, EDA, feature engineering, and ML model |
| **Topps_NBA_Print_Run_Prediction_Project.pdf** | Project summary exported from Notion |
| **README.md** | High-level project overview |

---

## 🙌 Acknowledgments

This project is part of a personal analytics portfolio exploring sports cards demand forecasting and applied machine learning.

---

## ⭐ If you find this useful…

Feel free to star the repo or connect with me on LinkedIn!
