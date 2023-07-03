## CSI500_Quant_Strategy

### Highlights
1. Only based on daily <open，high，low，close，volunme，amount> data
   
2. All parameters are based on grid search or the sub nerual network inferring/learning, quite automated

3. Selecting factors may easily cause unavoidable overfitting, we chose it because it perform well in the history. In my cases, all the factors are fixed before 2021-12, which means this factor will not influence 2021-12 to now

### Experiment Result

**1. Long-term Backtesting Result**

cumsum alpha: top 20% equal weighted - csi500; top 20% equal weighted - tail 20% equal weighted

![Image text]([https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/1.png](https://github.com/Neural-Finance/CSI500_Quant_Strategy/blob/main/CSI500_Long-term%20Backtesting.png))




### Input X and Output Y
![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/1.png)

![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/2.png)

**Lenet (A kind of CNN network structure)**

I want to mention that, sometimes, 1*m kernels will be more helpful in this task, because it's more like a time series operation. And the second point is that, I know GNN is very hot nowadays, however, you should know the relationship between different stocks. If you are pretty sure about it, then you should use GNN here. If you want to freely learn their relationship, both in time series or cross section relationship, then the tradtional CNN will be a better choice.

![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/5.png)

### Experiment Result
