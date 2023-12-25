# Dense Neural Networks to forecast stock returns

### For obvious reasons, I won't describe the specific architecture and feature engineering applied (nor allow to deduce it from the code). I'd rather keep it to myself. However, I will show the results obtained from it.
### There's no survivorship nor look-ahead bias, and it's been tested live to guarantee the validity of its results.
### The (exclusively) stocks in the portfolio, with no use of leverage and long-only positions, are equally weighted to obtain the result of such portfolio in each period.
### The prediction strategy has been trained and tested from short to long-term horizons (1/3/6/12 months into the future) for almost each month from 1991 till 2022. So there are 4 different models, one trained to predict 1 month ahead, another for 3 months ahead, and so on.
### The graphs shown below correspond to 1 model (3m horizon), as it would be too extensive to show graphs for each individual horizon. Even though graphs would be available for each of the 4 different horizons, only one is shown. However, some of the results from these 4 strategies plus the combination of them will be detailed further below the graphs.
### The graphs below is just 1 example that isn't the best strategy, that is the one with the best results (in terms of IR, annual return, lowest losses).


### Graphs (for 3m horizon predictions of individual stocks that make up an equally-weighted portfolio)

* The correlation between my portfolio and benchmark returns is yet positive, but lower than 1; therefore, its performance isn't tied to market movements.
Correlation Df 3m
        Ind_B  Dif_Per
Ind_P   0.61     0.88
Ind_B   1.00     0.17

These 2 graphs show I beat the benchmark (SPX) more than half of the time. I have negative returns almost a third of the time. I have an IR of 0.2 (vs SPX), an annualized return of 13%, and a maximum loss of 46% (in a 3-month period).
![image](https://github.com/MatiGrinberg/Equity_Prediction/assets/45952871/09dffb5c-1005-44ca-b1b6-ddd7fcb3709d)
![image](https://github.com/MatiGrinberg/Equity_Prediction/assets/45952871/7dc57096-57a2-471c-af33-b95cd27b9a93)
As the probability of including a stock in my portfolio increases, so does the return 3m ahead.
![image](https://github.com/MatiGrinberg/Equity_Prediction/assets/45952871/955c11c8-b4ac-455c-8c8e-750c232b3c6e)
The two graphs that follow show the evolution of the portfolio as I test its performance over time and accumulate its returns from each date.
![image](https://github.com/MatiGrinberg/Equity_Prediction/assets/45952871/6c9d2fc5-7519-48c9-96d4-bb60f950b9e7)
![image](https://github.com/MatiGrinberg/Equity_Prediction/assets/45952871/1acfb3dc-1585-4cf1-8140-4ffab3945b65)

### (annualized) Information Ratios (IR vs SPX)
"Only" refers to vanilla portfolios, e.g., picking stocks thinking 1 or 3m ahead and measuring their performance versus SPX in that same timeframe (used for the prediction). So, there's a coincidence in timeframe between prediction and turnover.
"Any_Pred" means a portfolio made up of stocks picked by any of the 4 models (either by the model forecasting stocks 1/3/6/12m ahead), but the turnover and therefore its performance measurement could be every 1m or 3m. Remember, all stocks, no matter if they were picked by one model or the other, are equally weighted.
"Target_3_Turn_1" is a portfolio made up of stocks picked via prediction 3m ahead, but with a monthly turnover.
"Avg_Strategy" assumes that every month, I allocate 25% of my portfolio weight to each of the 4 possible strategies, which, in turn, make their own portfolios with their individual 1m returns.

Only_1_SPX: 0.2
Only_3_SPX: 0.2
Any_Pred_1_SPX: 0.3
Any_Pred_3_SPX: 0.3
Targ_3_Turn_1_SPX: 0.2
Avg_Strat_1m_SPX: 0.6

These are all the types of strategies, but obviously, there are more results to show that I'll skip for now, as I think this is sufficient to prove the validity of my technique.
