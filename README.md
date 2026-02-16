📊 Investment Decision Analysis Using Bayesian Networks

🧠 Project Summary

This project models a high-stakes investment decision under discrete uncertainty using Bayesian Decision Networks implemented in Netica.
An individual investor must determine how to allocate a $1,000,000 portfolio between stocks and bonds while accounting for multiple layers of uncertainty, including:
- Stock market performance
- Bond yields
- Interest rates
- Geopolitical risk
- Probability of a market crash

The objective is to maximize expected portfolio return (utility) while considering risk tolerance and optional financial advice.

🎯 Problem Statement

An investor must choose among multiple asset allocation strategies:
- 90% Stocks / 10% Bonds
- 90% Bonds / 10% Stocks
- 70% Stocks / 30% Bonds
- 70% Bonds / 30% Stocks

Additionally, the investor can:
- Pay $15,000 for financial advice (market analysis)
- Adjust risk exposure after observing economic signals

Because future market conditions are uncertain, the investor uses Bayesian analysis to update beliefs based on observed information and determine the allocation that maximizes expected return.

The decision must balance:
- Expected returns
- Risk exposure
- Cost of information
- Sensitivity to geopolitical and economic factors

🛠 Methodology
The decision problem is modeled using an Influence Diagram constructed in Netica, incorporating:

🔹 Decision Nodes
- Market Allocation
- Pay for Financial Advice
- Risk Adjustment

🔹 Chance (Uncertainty) Nodes
- Stock Market Performance
- Bond Yields
- Central Bank Interest Rates
- Geopolitical Risk
- Market Crash Probability
- Market Analysis Result

🔹 Utility Node
Portfolio Return is defined as:

𝑈 = 1,000,000[(𝑅𝑒𝑡𝑢𝑟𝑛𝑠𝑡𝑜𝑐𝑘𝑠)(𝑊𝑒𝑖𝑔ℎ𝑡𝑠𝑡𝑜𝑐𝑘𝑠)+(𝑅𝑒𝑡𝑢𝑟𝑛𝑏𝑜𝑛𝑑𝑠)(𝑊𝑒𝑖𝑔ℎ𝑡𝑏𝑜𝑛𝑑𝑠)]−15,000 (if advice chosen)

​
Probabilities were derived using:
- Historical financial data
- Treasury interest rate statistics
- Economic forecasts
- Subjective expert judgment

📈 Key Results
The optimal strategy determined by the Bayesian model is:
- Do NOT pay for financial advice
- Maintain current risk allocation
- Invest 70% in Stocks and 30% in Bonds

Bayesian Network
![Bayesian_Network](images/Bayesian_Network_Netica.png)

💰 Expected Portfolio Return:

$67,340.50

This strategy maximizes expected utility under the modeled uncertainties.

🧩 Influence Diagram Structure
The model captures:
- Information flow from uncertainties to decisions
- Conditional probability relationships
- Trade-offs between risk and expected return
- Value of information analysis

The Bayesian network structure allows dynamic updating of beliefs when new evidence is introduced.
