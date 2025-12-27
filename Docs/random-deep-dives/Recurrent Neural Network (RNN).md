An **RNN** is a neural network designed to process **sequences** (text, time series, signals) by maintaining a **hidden state** that carries information forward through time.

![[Pasted image 20251226190634.png]]

Instead of treating each input independently, an RNN updates a hidden state:

$$h_t = f(W_xx_t + W_hh_{t-1})$$

The hidden state acts as a summary of everything the model has learned up until time t. But the limitations is that all information must fit in one context vector. The solution later comes from giving the models the idea of "attention" which means they can look at all of the hidden states.


This came up when learning about seq2seq which is a model for transforming sequences from one to another. In this model architecture it used RNN as an encoder and a decoder. [[Understanding Foundational Models]]
