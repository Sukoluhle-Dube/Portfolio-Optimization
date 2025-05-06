# Portfolio Optimization and Efficient Frontier

This project demonstrates portfolio optimization using Python and libraries like NumPy, Pandas, Matplotlib, and SciPy. It calculates optimal portfolio weights to maximize returns while minimizing risk, and visualizes the Efficient Frontier.

## Functionality

1. **Data Input:**
   - Defines a list of assets (e.g., AAPL, MSFT, GOOGL, AMZN, TSLA).
   - Uses hypothetical or fetched (using `yfinance`) expected returns and a covariance matrix for these assets.
   - You can modify these inputs to analyze different portfolios.

2. **Portfolio Optimization:**
   - Employs the Sharpe Ratio as the optimization metric.
   - Uses `scipy.optimize.minimize` to find the optimal portfolio weights.
   - Constraints ensure weights sum to 1 (full investment) and prevent short selling (weights between 0 and 1).

3. **Performance Metrics:**
   - Calculates and displays:
     - Expected return over a specified investment duration.
     - Annualized return.
     - Annualized volatility (risk).
     - Sharpe Ratio.
     - Potential profit and loss based on initial capital.

4. **Efficient Frontier:**
   - Generates the Efficient Frontier by simulating numerous portfolios with random weights.
   - Plots the Efficient Frontier, with points colored by their Sharpe Ratios.

## How to Use

1. **Installation:**
   - Ensure you have the necessary libraries installed:
