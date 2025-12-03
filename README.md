## 📈 Macro-Driven FX Trading Strategy: USD/INR with Bloomberg Data
A quantitative trading strategy for USD/INR based on macroeconomic indicators, implemented in Python using synthetic Bloomberg-style data. The strategy incorporates interest rate differentials and Purchasing Power Parity (PPP) analysis to generate trading signals.

# 📁 Project Structure
Macro_Driven_FX_Trading_Strategy_USD_INR_with_Bloomberg_Data/
├── main.py                          # Core trading strategy implementation
├── data_generator.py                # Synthetic market & macro data generation
├── market_macro.csv                 # Combined macroeconomic dataset
├── usd_inr.csv                      # USD/INR spot rates
├── rbi_repo.csv                     # RBI repo rate data
├── fed_funds.csv                    # Fed funds rate data
├── india_cpi.csv                    # India CPI data
├── us_cpi.csv                       # US CPI data
└── README.md                        # Project documentation
# 🧠 Strategy Overview
The strategy uses:
1) Interest Rate Differential (RBI Repo vs. Fed Funds Rate)
2) Purchasing Power Parity (PPP) analysis using CPI indices for India and the US
3) Rule-based entry/exit signals for USD/INR spot trading

# 📊 Performance Summary (Backtest: 2020–2023)
Metric	Value
Total Return	-8.82%
Annualized Return	-1.58%
Sharpe Ratio	-1.90
Maximum Drawdown	-9.53%
Win Rate	43.83%
Total Trades	308
Daily 95% VaR	-0.43%
# Risk Metrics (95% Confidence)
Historical VaR: -4.78%

Parametric VaR: -5.12%

Monte Carlo VaR: -5.17%

# 🔧 Installation
git clone https://github.com/your-username/usd-inr-macro-trading.git
cd usd-inr-macro-trading
pip install pandas numpy matplotlib
# 🚀 Usage
1. Generate Synthetic Data
bash
python data_generator.py
2. Run the Strategy
python
python main.py
3. View Results
The strategy will output:

Performance report

Risk metrics

Visualized results (PnL, drawdown, trade signals)

# 📈 Key Features
Synthetic Data Generation: Realistic USD/INR, RBI repo, Fed funds, and CPI data

Multi-Factor Model: Combines interest rates and inflation for signal generation

Risk Management: Includes VaR calculations (Historical, Parametric, Monte Carlo)

Comprehensive Backtesting: Detailed performance and risk reporting

Visualization: PnL, drawdown, and trade visualization

# 📊 Data Fields
Column	Description
date	Business date
usd_inr	Synthetic USD/INR spot rate
rbi_repo	RBI repo rate (monthly steps)
fed_funds	Fed funds rate (monthly steps)
cpi_india	India Consumer Price Index
cpi_us	US Consumer Price Index
🧪 Example Output
The strategy generates:

Equity curve

Drawdown chart

Trade entry/exit markers

Macro factor plots

⚠️ Disclaimer
This is a research and educational project. The synthetic data is randomly generated and does not represent real market conditions. Not intended for live trading.

📄 License
MIT
