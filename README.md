# eece490-ps3p4
Submission for EECE490 Problem 4, PS3.

This notebook demonstrates using a fully-connected neural network on the bank churn binary classification dataset located at Kaggle [here](https://www.kaggle.com/datasets/cybersimar08/binary-classification-of-bank-churn-synthetic-data).

The architechture is simple: 
* An input layer, consisting of 64 neurons.
* A hidden layer, consisting of 32 neurons.
* An output layer, consisting of 1 neuron.
  
ReLU functions are used as activations for the first two layers. A sigmoid function is used at the output layer for classification purposes. Each layer is fed into a dropout of sensitivity 0.5 to make the network resistant to overfitting.

The network is trained with a simple stochastic gradient descent optimizer using binary cross entropy loss, which performed the best when compared with Adam optimizers or other loss kinds. The model achieves 79% validation set accuracy.
