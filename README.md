# Rough-Volatility-Models-Deep_Learning

### What are volatility models?
-----------------------------------------------------------------------------------------------------------------------------------------
Volatility models, more broadly, refer to mathematical models used to describe and forecast the volatility of financial assets.
<br>Volatility represents the degree of fluctuation or uncertainty in the price of an asset over a given period. <br>Accurate volatility modeling is crucial for risk management, option pricing, and portfolio optimization.

### Stochastic Volatility Models
-----------------------------------------------------------------------------------------------------------------------------------------
Stochastic volatility models are mathematical models used in finance to describe the dynamics of asset prices and their associated volatilities.<br>
In stochastic volatility models, the volatility process is typically described by a stochastic differential equation (SDE). The volatility process can exhibit various characteristics, such as mean-reversion, jumps, or regime-switching, depending on the specific model employed.

### Rough Volatility Models
-----------------------------------------------------------------------------------------------------------------------------------------
Rough volatility models are a class of stochastic volatility models that aim to capture the long-term memory and roughness observed in financial volatility. These models depart from traditional models, such as the Heston model or the local volatility model, by incorporating fractional Brownian motion or fractional stochastic volatility processes.<br>
In rough volatility models, the volatility process is typically characterized by a fractional stochastic differential equation (SDE) driven by fractional Brownian motion or fractional Lévy processes. These models allow for flexible and non-Markovian dynamics, capturing the time-varying and persistent nature of volatility.

## Structure

- The notebook **SPX-Parser.ipynb** demonstrates how to parse the raw data retrieved from https://www.cboe.com/, to get the joint distribution of moneyness M and time to maturity T, and draw randomly 1000000 pairs from the estimated distribution.
- The notebook **Data-Generator.ipynb** demonstrates how to generate labeled dataset of Heston Model and rBergomi Model for training the IV prediction Neural Network.
- The notebook **Deep-Calibration.ipynb** demonstrates how to preprocess synthetic data, build and train Neural Networks, and use them to predict IV.
- The notebook **CNN-calibration.ipynb** demonstrates the whole pipeline of the second paper.


Implied Volatility(IV) is a financial metric used in options pricing. It represents the market's expectation of the future volatility of the underlying asset based on the observed prices of options.
