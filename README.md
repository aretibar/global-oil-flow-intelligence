🌍 Global Oil Flow Intelligence
📊 Supply Signal Engineering & Price Interaction Analysis
📌 Project Overview

This project simulates an oil market intelligence workflow inspired by trade flow and energy analytics platforms.

Using country-level crude production data and Brent price series, the objective is to engineer interpretable supply-side signals that may indicate tightening or disruption in global oil markets.

The analysis focuses on:

📈 Rolling export momentum

🚨 Statistical supply shock detection

💰 Supply–price interaction signals

📊 Visual interpretation of market behavior

🎯 Business Objective

Energy trading desks and intelligence platforms monitor supply trends to detect:

⛽ Production slowdowns

⚠️ Structural supply shocks

🔥 Potential tightening conditions

📉 Early indicators of price reaction

This project builds a simplified statistical framework to simulate that workflow.

📊 Data Sources

🌎 Simulated country-level crude production

Saudi Arabia

USA

Russia

Iraq

UAE

💵 Simulated daily Brent crude prices

(Designed to replicate real-world energy data structure for portfolio demonstration purposes.)

🛠 Tech Stack

🐍 Python

🐼 Pandas

🔢 NumPy

📈 Matplotlib

📓 Jupyter Notebook

📈 Methodology

1️⃣ Global Production Aggregation

Daily country production aggregated into total global supply.

2️⃣ Rolling Momentum Indicator

30-day rolling mean applied to smooth volatility.

Momentum defined as:
pct_change(rolling_30_day_production)

This removes short-term noise and highlights structural shifts.

3️⃣ 🚨 Statistical Supply Shock Detection

Supply shock events defined as:
momentum < mean - 2 * standard_deviation
This identifies statistically significant negative supply deviations.

4️⃣ 🔥 Tight Supply Signal

Signal triggered when:

Production momentum < 0

Brent price daily return > 0

This simulates price reacting to tightening supply conditions.

📌 Key Findings

🚨 34 statistically significant supply shock events detected.

🔥 Tight supply signal occurred rarely (1 event in synthetic dataset).

🔗 Correlation between production momentum and Brent price was weak, suggesting lag effects or additional macro drivers.

📊 Rolling indicators improve interpretability versus raw production data.

🧠 Future Improvements

📥 Use real EIA / OPEC production datasets

🏦 Add inventory data (OECD stocks)

⏳ Incorporate lagged correlation analysis

📉 Add structural break detection

🌐 Deploy as interactive dashboard (Streamlit)

🚀 How to Run

1️⃣ Clone the repository

2️⃣ Install dependencies:

pip install -r requirements.txt


3️⃣ Open:

notebooks/01_oil_flow_signals.ipynb


4️⃣ Run all cells

💡 Why This Matters

Energy markets are driven by expectations about supply and demand.

This project demonstrates how statistical signal engineering can transform raw production data into interpretable market intelligence indicators.

It showcases:

🧮 Time series analysis

📊 Rolling metrics

🚨 Signal design

💼 Business interpretation

🌍 Energy market understanding
