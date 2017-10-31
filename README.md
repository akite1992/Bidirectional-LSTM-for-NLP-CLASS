# Bidirectional-LSTM-for-NLP-CLASS
This is the code for final project of Natural Language Processing Class at MIT in 2016.

The main purpose is to implement and train a bidirectional LSTM for a sequence to sequence mode: generate regular expression from human language.

The code is based on an open-source package: https://github.com/harvardnlp/seq2seq-attn.

The main modification by me is the following:

1. In newbrnn_train.lua, I modified the original implementation of bidirectional LSTM.  Before, two hidden states at each step from two direction 
are just summed to get a new hidden state.  Here instead, I concatenate them to a larger hidden state for usage in attention mechanism during 
decoder.

2. Train Bi-LSTM in a dataset which generate regular expression form human language.
