# Introduction
In this notebook, I train an image captioning model roughly based on the injection model in [Where to Put the Image in an Image Captioning Model](https://arxiv.org/abs/1703.09137), except the text "encoder" is a transformer encoder instead of an RNN, and the model is trained to predict the input text sequence shifted by 1 (like in a sequence to sequence model) rather than only the next character in the input sequence. The model is trained on Flikr8k. 

# To do
I am still training the model. I plan to evaluate it usiing BLEU scores.