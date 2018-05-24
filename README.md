# NN-Checkpoint
LSTM classification of colleges using Wikipedia entries

The IPython Notebook grabs the text of 100 Wikipedia articles, and tries to predict the average income quintile of its 
students from the text.

The architecture of the network is one embedding layer to process input, one 20-cell LSTM recurrent layer, and one tanh 
Dense perceptron network, which then maps to the output quintile. The model only takes a few minutes to train on my 2014 
Macbook Air, but performance is very poor, and I'm unsure that learning has occurred, since the validation set accuracy 
is stable at .80 across all epochs. 

A task as subtle as this one is difficult for humans, I suspect that carrying out this task to obtain meaningful results would
require far more data than we have available, and even then would might be too subtle for an ANN to process. Future steps might 
include using an automated reasoning system in conjunction with an RNN like this one, or repeating the task with more data.

Done for Prof. Rogers EECS 397: Data Science Course.
