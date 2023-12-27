# Results of all strategies tried
These results are not definitive and are expected to be improved in the near future.

## IRs vs SPX

The explanation of what each of these strategies mean was already provided in the previous ReadMe file. Now, I've decided to display all results. You can observe that in all cases, I achieved a high IR versus SPX. All IRs in this document are annualized.

| Strategy             | Value  |
|----------------------|--------|
| Only_1_SPX           | 0.2    |
| Only_3_SPX           | 0.2    |
| Only_6_SPX           | 0.4    |
| Only_12_SPX          | 0.2    |
| Any_Pred_1_SPX       | 0.4    |
| Any_Pred_3_SPX       | 0.3    |
| Any_Pred_6_SPX       | 0.3    |
| Any_Pred_12_SPX      | 0.2    |
| Targ_3_Turn_1_SPX    | 0.3    |
| Targ_6_Turn_1_SPX    | 0.7    |
| Targ_6_Turn_3_SPX    | 0.5    |
| Targ_12_Turn_1_SPX   | 0.5    |
| Targ_12_Turn_3_SPX   | 0.3    |
| Targ_12_Turn_6_SPX   | 0.1    |
| Avg_Strat_1m_SPX     | 0.7    |

## IRs vs NDX

In many cases, though not all, there's a decent (0.2) or even high (0.4) Information Ratio (IR) versus NDX, which has significantly outperformed the SPX in recent decades (the NDX's IR versus SPX is around 0.4). All IRs in this document are annualized.

| Strategy             | Value  |
|----------------------|--------|
| Only_1_NDX           | -0.0   |
| Only_3_NDX           | 0.0    |
| Only_6_NDX           | 0.2    |
| Only_12_NDX          | -0.0   |
| Any_Pred_1_NDX       | 0.1    |
| Any_Pred_3_NDX       | -0.0   |
| Any_Pred_6_NDX       | 0.0    |
| Any_Pred_12_NDX      | -0.1   |
| Targ_3_Turn_1_NDX    | 0.0    |
| Targ_6_Turn_1_NDX    | 0.4    |
| Targ_6_Turn_3_NDX    | 0.2    |
| Targ_12_Turn_1_NDX   | 0.2    |
| Targ_12_Turn_3_NDX   | -0.0   |
| Targ_12_Turn_6_NDX   | -0.1   |
| Avg_Strat_1m_NDX     | 0.3    |

## Annualized Return for all strategies

Equity indices have returned roughly 10 to 14% annually, while some of my strategies achieved an annualized return of around 20%.

| Strategy             | Value  |
|----------------------|--------|
| Any_Pred_1           | 0.14   |
| Any_Pred_3           | 0.14   |
| Any_Pred_6           | 0.14   |
| Any_Pred_12          | 0.13   |
| Only_1               | 0.13   |
| Only_3               | 0.15   |
| Only_6               | 0.18   |
| Only_12              | 0.13   |
| Targ_3_Turn_1        | 0.14   |
| Targ_6_Turn_1        | 0.23   |
| Targ_6_Turn_3        | 0.21   |
| Targ_12_Turn_1       | 0.19   |
| Targ_12_Turn_3       | 0.14   |
| Targ_12_Turn_6       | 0.12   |
| Avg_Strat_1m         | 0.19   |

## Maximum Loss for all strategies

Losses are measured within the timeframe/horizon of each strategy. For instance, 'Any_Pred_1' displays the maximum loss for a strategy that trades monthly, while 'Any_Pred_3' shows the same for a strategy that trades quarterly. The majority of these losses occurred by Sep-08 before the Lehman moment. However, when you examine losses for each individual strategy, they're not as high as the maximum and typically hover around a maximum of 20% when considering consecutive months. Within a single month, the losses would be much less. Essentially, I didn't observe any significant difference in the losses one might suffer compared to adopting a passive strategy of buying the SPX or NDX.

| Strategy             | Value  |
|----------------------|--------|
| Any_Pred_1           | -0.43  |
| Any_Pred_3           | -0.43  |
| Any_Pred_6           | -0.48  |
| Any_Pred_12          | -0.52  |
| Only_1               | -0.4   |
| Only_3               | -0.46  |
| Only_6               | -0.41  |
| Only_12              | -0.65  |
| Targ_3_Turn_1        | -0.44  |
| Targ_6_Turn_1        | -0.45  |
| Targ_6_Turn_3        | -0.45  |
| Targ_12_Turn_1       | -0.29  |
| Targ_12_Turn_3       | -0.46  |
| Targ_12_Turn_6       | -0.6   |
| Avg_Strat_1m         | -0.32  |
