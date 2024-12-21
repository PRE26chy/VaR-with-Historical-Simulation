# VaR-with-Historical-Simulation
Value at risk(VaR) is a statistical measure that represents the maximum loss of a portfolio over a specified period for a given confidence level. Risk Managers use VaR to understand and control the level of risk exposure to a specific position or whole portfolio and use them to measure firm-wide risk exposure. The two main components of Var are: 

1. Confidence Interval
2. Time Period

Var is expressed as a dollar amount and confidence level. For ex, “There is a 5% probability that the portfolio will lose $Y over the next X days.”

There are three main ways of computing VaR 
1. Variance-Covariance(Parametric Method)
2. Historical Simulation(Non-Parametric Method)
3. Monte-Carlo Simulations

In this notebook, I have calculated the VaR of a portfolio consisting of 5 stocks:
1. Vanguard Total Bond Market Index Fund ETF('BND')
2. SPDR S&P 500 ETF Trust ('SPY')
3. SPDR Gold Trust ('GLD')
4. Invesco QQQ Trust ('QQQ')
5. Vanguard Total Stock Market Index Fund ETF ('VTI')

Using Historical Simulation. I have calculated 50-day VaR at both 99% and 95% confidence interval.
For this purpose, I fetched past 10 year returns of the portfolio.  

In the historical simulation method, we do not assume any distribution. We calculate Var using the historical returns that are sorted from low to high. The method is extremely simple to calculate and can be explained to people with no risk knowledge. We do not have to make any assumptions and they can also be used in case of non-linear estimates.

The method assumes that future outcomes can be determined through past returns, which highlights the major drawback of this method. Technological, regulatory, etc. changes can change the direction of future outcomes. The historical simulation method can be slow to react to such a changing market environment.
