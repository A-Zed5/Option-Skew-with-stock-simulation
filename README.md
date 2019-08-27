# Option-Skew-with-stock-simulation

Simulate series of stock paths to create a stock distribution with non-constant volatility as a way of illustrating why volatiltiy skew exists. 

The code simulates a stock using GBM with a default volatility of 15 on an arbitrary $100 stock, howevever, if the stock falls below an arbitrary threshold ($90) volatility spikes to 90. The resulting distribution is noticeably skewed (there are extreme outliers to the downside) and this ultimatley must be reflected in any options on this hypothetical stock. 

There's some graphs to illustrate the stock distribution, and the distribution of realized volatility. 

Finally the code backs out an "options price" by using an average of the payoffs, and then calculates an implied volatility using BSM. 

Running the code with and without the stochastic element illustrates the differences in the resutling distribution and the effects on option prices and skew
