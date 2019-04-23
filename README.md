# pltnn
try to show very simple neural networks interactively with different activations (plot neural networks)

这是一个非常简单的用于从直观上理解神经网络为何可以进行分类的可视化交互式 matplotlib 小程序。目前它可以提供如下几种模型的可视化：

## 4 种基本模型

1. 单层单节点，对应 plot_neuron_11
```
#   w1*x + w0
# x----------->y
```

![1 输入 1 输出](https://github.com/llinjupt/pltnn/blob/master/11.png)


2. 2 层单节点，对应 plot_neuron_111
```
#  w11*x1 + w10  a1*w21 + w20 
# x1----------->a1--------->y1
```

![2 层 1 输入 1 输出](https://github.com/llinjupt/pltnn/blob/master/111.png)

3. 单层 2 输入 1 输出，对应 plot_neuron_21   
```
#   w11*x1 + w12*x2 + w10 
# x1----------+
#             |->y
# x2----------+
```

![2 输入 1 输出](https://github.com/llinjupt/pltnn/blob/master/21.png)

4. 2 层，2 输入 1 输出，对应 plot_neuron_211
```
# x1----------+
#             |------>a------->y
# x2----------+
```

![2 层 2 输入 1 输出](https://github.com/llinjupt/pltnn/blob/master/211.png)

## 如何使用

使用非常简单，直接打开相应注释行即可：

```
  if __name__ == "__main__":
      pltnn = pltNN(type='sigmoid')
      #pltnn.plot_neuron_11()
      #pltnn.plot_neuron_111()
      pltnn.plot_neuron_21()
      #pltnn.plot_neuron_211()
```

## 支持的激活函数

初始化 pltNN 类可以传入 type 参数指定使用的激活函数，目前支持：

'logistic', 'relu' 和 'tanh'，当然扩展它们非常容易。
