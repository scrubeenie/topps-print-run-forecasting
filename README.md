📘 Topps Print Run Forecasting (NBA + MLB Expansion Project)

Machine learning project analyzing and forecasting Topps Now print runs using:

Feature engineering

Exploratory data analysis

Random Forest regression

Log-transformed modeling for skewed distributions

Visualization (matplotlib, seaborn)

Future Power BI dashboards

This project builds a predictive framework for understanding how factors such as rookies, superstars, multi-player cards, team market size, and rare inserts influence daily sports card print runs.

🔍 Project Overview

Topps Now cards have highly variable print runs driven by real-time market demand.
This project answers:

👉 Can we predict print runs using publicly available card metadata?
👉 Which card attributes most strongly influence demand?

🧠 Current Model Performance

Using a Random Forest Regressor with engineered features:

Metric	Score
R² Score	0.587
Log MAE	0.741
Log RMSE	0.983

This means the model explains ~59% of the variance in print runs — strong given the small dataset and volatile nature of Topps Now card demand.

🔧 Feature Engineering Included

The following features were created and tested:

IsRookie – Rookie Card flag

IsVet – Veteran flag

IsSuperstar – Curry, LeBron, Luka, Jokic, Giannis, Wembanyama, SGA

SPInserts – Short Print indicator

HasAutoRelic – Autograph or relic included

TeamTier – 1–7 tiering of NBA markets based on popularity & market size

IsMultiPlayer – Multi-player card indicator

📊 Exploratory Visuals (Jupyter Notebook)

The notebook includes:

Distribution of print runs

Rookie vs Vet print run comparison

Short print vs non-SP analysis

Superstar effect on demand

Team tier analysis

Actual vs Predicted scatterplot

Feature importance chart

🤖 Machine Learning Workflow

Data cleaning + normalization

Manual mapping of player tiers & superstar groups

Log transformation of target (Print Run)

Train/test split

Hyperparameter-tuned Random Forest

Evaluation on log scale

Back-transforming predictions for interpretability

📁 Repository Structure
📦 topps-print-run-forecasting
 ┣ 📄 README.md
 ┣ 📓 Topps_Now_NBA.ipynb               ← Full ML notebook
 ┣ 📄 Topps_Now_NBA_Print_Run_Summary.pdf (Notion export)
 ┗ 📂 /data (coming soon)


Power BI visual dashboards will be added next.

🚀 Roadmap
Short-Term

Add MLB Topps Now dataset

Compare NBA vs MLB print run drivers

Publish Power BI dashboards to GitHub & LinkedIn

Add model comparison (XGBoost, CatBoost, ElasticNet)

Medium-Term

Deploy interactive dashboard using:

Streamlit

Plotly Dash

Power BI Web Embed

Create a combined multi-sport forecasting model

Long-Term

Train large model across NBA, MLB, EPL, WWE, and F1 Topps Now

Build ranking system for "Expected Demand Score"

Predict print runs immediately upon card release

📎 Documentation

📄 Project Summary (Notion)
(Publish link here once ready)

📓 Notebook:
Topps_Now_NBA.ipynb

🏀🌟 Why This Project Matters

Sports card analytics is an emerging field with limited open-source tooling.
This project demonstrates:

Real-world forecasting on a rapidly changing product

Business analytics mindset

End-to-end machine learning pipeline

Ability to translate domain expertise into features

Strong documentation + storytelling for portfolio use
