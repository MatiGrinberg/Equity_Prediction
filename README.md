# Dense Neural Networks to forecast stock returns

### For obvious reasons, I won't describe the specific architecture and feature engineering applied (nor allow to deduce it from the code). I'd rather keep it to myself. However, I will show the results obtained from it.
### There's no survivorship nor look-ahead bias, and it's been tested live to guarantee the validity of its results.
### The (exclusively) stocks in the portfolio, with no use of leverage and long-only positions, are equally weighted to obtain the result of such portfolio in each period.
### The prediction strategy has been trained and tested from short to long-term horizons (1/3/6/12 months into the future) for almost each month from 1991 till 2022. So there are 4 different models, one trained to predict 1 month ahead, another for 3 months ahead, and so on.
### The graphs shown below correspond to 1 model (3m horizon), as it would be too extensive to show graphs for each individual horizon. Even though graphs would be available for each of the 4 different horizons, only one is shown. However, the results from these 4 strategies plus the combination of them will be detailed further below the graphs.


### Graph 1
* The correlation between my portfolio and benchamrk returns is yet positive, but lower than 1, therefore its performance isn't tied to market movements.
  Correlation Df 3m
        Ind_B  Dif_Per
Ind_P   0.61     0.88
Ind_B   1.00     0.17
![image](https://github.com/MatiGrinberg/Equity_Prediction/assets/45952871/09dffb5c-1005-44ca-b1b6-ddd7fcb3709d)

### Graph 2


### Graph 3


### Information Ratios (IR)



