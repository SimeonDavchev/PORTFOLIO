## Portfolio Optimization with Efficient Frontier


#### Description:
This Jupyter notebook assists users in optimizing their investment portfolio by combining it with a risk-free asset. It offers a comprehensive tool that leverages historical stock price data, modern portfolio theory, and visualisation techniques to guide investment decisions.

#### Key Insights:
- **Mean-Variance Optimization (MVO):** This classic approach focuses on deriving a set of optimal asset weights to achieve desired portfolio returns with minimized risk.
- **Efficient Frontier:** Visual representation of the set of optimal portfolios offering the highest expected return for a defined level of risk.
- **Sharpe Ratio Maximization:** By maximizing this ratio, the tool identifies the portfolio with the best risk-adjusted return.
- **Capital Market Line (CML):** Demonstrates the risk-return trade-off for combining a risk-free asset with a risky portfolio.

#### Overview of Methods and Theory:
1. **Data Input:** Choose between a 'demo' mode with preset values or an 'interactive' mode for customized inputs.
2. **Data Collection:** Fetch real-time stock price data based on user-defined tickers and date ranges.
3. **Portfolio Optimization:** Employ MVO to determine the optimal mix of assets. The notebook calculates the efficient frontier, plots the CML, and identifies portfolios with maximum Sharpe ratios and minimum volatility.
4. **Output Analysis:** Visual representations and tables provide insights into the expected annualized return, volatility, and price of the optimized portfolios.
5. **Portfolio Composition:** Deep dive into how to best combine the optimized portfolio with a risk-free asset.

#### Setup:
1. Install required libraries, including numpy, pandas, pandas_datareader, yfinance, scipy, and matplotlib.
2. Opt for either 'demo' or 'interactive' modes based on preference.

#### Usage:
1. Progressively move through each section of the notebook, following the provided instructions.
2. In 'interactive' mode, input relevant parameters when prompted.
3. Analyze the resulting visualizations and tables to inform your investment decisions.

#### Remarks:
- Maintain a stable internet connection for real-time data fetching.
- Long lists of stocks will take a long time to process, so opt in for the preset stock list or input one that is preferably under 100 stocks

#### **Disclaimer**: 
This notebook is developed for academic and project purposes only. It is not intended to provide, and should not be relied upon for, investment advice, recommendations, or endorsements. Investing in financial markets involves risks, and you should always consult with a professional financial advisor before making any investment decisions. 