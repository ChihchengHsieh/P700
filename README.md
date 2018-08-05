# Siamese-Network for analysing graphs

## Grid Graph (a kind of Planar graph is used in this case)
#### Start from 1 to 20 (20 nodes)
![](https://github.com/ChihchengHsieh/P700/blob/master/Img/Graph.png?raw=true) 

## Data Generation
![](https://github.com/ChihchengHsieh/P700/blob/master/Img/DataGeneration.png?raw=true)

## Network Architecture
![](https://github.com/ChihchengHsieh/P700/blob/master/Img/P700St.png?raw=true)

## NELU LSTM
#### NELU has been implemented.
[[NALU Paper](https://arxiv.org/pdf/1808.00508.pdf)]
![](https://github.com/ChihchengHsieh/NALU-and-Applying-on-LSTM/blob/master/NALU.png?raw=true)

# Result from Pytorch
The learning rate decay has been implemented in this model.
We can see the model can only classify the data it has seen. And the accuracy on the validation set is not increasing.

![](https://github.com/ChihchengHsieh/P700/blob/master/Img/Train_HistEpoch.png?raw=true)

### After Applying the L2 Regularization, it still can't be solved

![](https://github.com/ChihchengHsieh/P700/blob/master/Img/Train_HistEpoch_0.2reg.png?raw=true)

# Result from tf.Keras

![](https://github.com/ChihchengHsieh/P700/blob/master/Old%20Models/Keras_Results/FullDataOnlyLSTM1lr0.0001.png?raw=true)


### However, this problem can be solved by using a simple algorithm (Graph_Alg) to create a graph.
#### Only few batch of training data can boost the accuracy on the validation set to 100%

![](https://github.com/ChihchengHsieh/P700/blob/master/Img/Graph_algo_hist.png?raw=true)


