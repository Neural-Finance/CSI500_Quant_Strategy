# CSI500_Quant_Strategy

### Highlights
1. Only based on daily <open，high，low，close，volunme，amount> data
   
2. All parameters are based on grid search or the sub nerual network inferring/learning, quite automated

3. Selecting factors may easily cause unavoidable overfitting, we chose it because it perform well in the history. In my cases, all the factors are fixed before 2021-12, which means this factor will not influence 2021-12 to now

### Project Structure
```
Main.py --You can run it to train the network and test the data.
```

```
Data_processing.py --Built the figure data
```

```
Querry.py --a sub function for Data_processing, here, you can put in a formula, which produces x and y
```

```
Lenet.py --The neural network model structure (Tensorflow 1.3)
```

```
hyper_parameters.py --all the hyper-parameters
```

### Input X and Output Y
![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/1.png)
![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/2.png)

**Lenet (A kind of CNN network structure)**

I want to mention that, sometimes, 1*m kernels will be more helpful in this task, because it's more like a time series operation. And the second point is that, I know GNN is very hot nowadays, however, you should know the relationship between different stocks. If you are pretty sure about it, then you should use GNN here. If you want to freely learn their relationship, both in time series or cross section relationship, then the tradtional CNN will be a better choice.

![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/5.png)

### Experiment Result

**Valid Gradient Descent**

![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/3.png)

**Prediction and Real**

![Image text](https://github.com/Neural-Finance/Cross_sample_financial_feature_engineering/blob/master/fig/4.png)

This result can be much better if you train it with GPU. I show the result on my laptop, thus, it hasn't got enough training. However, as you can see, our method sucessfully learns the rank() operator. This framework can help you learn the relationship between different stocks. **If it's helpful, please give me a star, thanks.**
