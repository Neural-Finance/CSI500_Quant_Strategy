## CSI500_Quant_Strategy

### Highlights
1. **Only based on daily <open，high，low，close，volunme，amount> data**, because I have no Wind Database nearby. If I can add some basic quality factors, wind consensus factors into it, the return will be 20% higher, better sharpe ratio, smaller max-drawdown, you can go for details in [https://personal-web-nf101.github.io/My_quant_strategy]. If you want to know how this strategy perform in CSI300 Index, CSI500 Index, Equity Tilt Index Product, you can go for details in [https://personal-web-nf101.github.io/Daily_Price_and_Volume_Alpha].
   
2. All parameters are based on grid search or the sub nerual network inferring/learning, quite automated.

3. Selecting factors may easily cause unavoidable overfitting, we chose it because it perform well in the history. **All the factors are fixed before 2021-12, which means I change nothing, just let this strategy run from 2021-12 to now.**

### Experiment Result

**1. Long-term Backtesting Result**

cumsum alpha: top 20% equal weighted - csi500; top 20% equal weighted - tail 20% equal weighted

![Image text](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_Long-term%20Backtesting.png)

**2. All Factors Backtesting Result**

Show the performance of some compounded alpha factors, some of them are a single neural network, has sub network to infer parameters or decide how to combine things

![Image text](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_all_factors%20Backtesting.png)

**3. Summary of Backtesting Result**

All the indicators are calculated afterfee, this fee is decent.

![Image text](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_Table%20Backtesting.png)

**4. 2023 YTD Backtesting Result**

![Image text](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_YTD%20Backtesting.png)

**5. 2023 YTD Backtesting Result Compared with Huaxia**

Huaxia Fund, its English name is the China Asset Management Fund, their CSI500 product (Blue) is almost the best among mutual fund industry (both suffer from bad trading environment and prefer low turnover strategy). I compare my half-way product with them (Red).

![Image text](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_compare_with_huaxia.png)

**Thanks for your attention! Please feel free to reach out, if you have any questions or interests! via alex.holla@foxmail.com** 
