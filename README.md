# pltnn
try to show very simple neural networks interactively with different activations (plot neural networks)

����һ���ǳ��򵥵����ڴ�ֱ�������������Ϊ�ο��Խ��з���Ŀ��ӻ�С����Ŀǰ�������ṩ���¼���ģ�͵Ŀ��ӻ���

4 �ֻ���ģ��
-------------

1. ���㵥�ڵ㣬��Ӧ plot_neuron_11
#   w1*x + w0
# x----------->y

2. 2 �㵥�ڵ㣬��Ӧ plot_neuron_111
#  w11*x1 + w10  a1*w21 + w20 
# x1----------->a1--------->y1

3. ���� 2 ���� 1 �������Ӧ plot_neuron_21   
#   w11*x1 + w12*x2 + w10 
# x1----------+
#             |->y
# x2----------+

4. 2 �㣬2 ���� 1 �������Ӧ plot_neuron_211
# x1----------+
#             |------>a------->y
# x2----------+

���ʹ��
-------------

ʹ�÷ǳ��򵥣�ֱ�Ӵ���Ӧע���м��ɣ�

'''
  if __name__ == "__main__":
      pltnn = pltNN(type='sigmoid')
      #pltnn.plot_neuron_11()
      #pltnn.plot_neuron_111()
      pltnn.plot_neuron_21()
      #pltnn.plot_neuron_211()
'''

֧�ֵļ����
--------------

��ʼ�� pltNN ����Դ��� type ����ָ��ʹ�õļ������Ŀǰ֧�֣�

'logistic', 'relu' �� 'tanh'����Ȼ��չ���Ƿǳ����ס�

ģ��ʾ��
--------------

![2 ���� 1 ���](https://github.com/llinjupt/pltnn/21.png)
