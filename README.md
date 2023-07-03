## CSI500_Quant_Strategy

### Highlights
1. **Only based on daily <open，high，low，close，volunme，amount> data**, because I have no Wind Database nearby. If I can add some basic quality factors, wind consensus factors into it, the return will be 20% higher, better sharpe ratio, smaller max-drawdown, you can go for details in (https://personal-web-nf101.github.io/My_quant_strategy). If you want to know how this strategy perform in CSI300 Index, CSI500 Index, Equity Tilt Index Product, you can go for details in (https://personal-web-nf101.github.io/Daily_Price_and_Volume_Alpha).
   
2. All parameters are based on grid search or the sub nerual network inferring/learning, quite automated.

3. Selecting factors may easily cause unavoidable overfitting, we chose it because it perform well in the history. **All the factors are fixed before 2021-12, which means I change nothing, just let this strategy run from 2021-12 to now.**

### Experiment Result

**1. Long-term Backtesting Result**

cumsum alpha: top 20% equal weighted - csi500; top 20% equal weighted - tail 20% equal weighted

![Image text](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_Long-term%20Backtesting.png)

**2. All Factors Backtesting Result**

cumsum alpha: top 20% equal weighted - csi500; top 20% equal weighted - tail 20% equal weighted

![Image text](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_all_factors%20Backtesting.png)
