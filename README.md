# Introduction
In this notebook, I train an image captioning model roughly based on the injection model in [Where to Put the Image in an Image Captioning Model](https://arxiv.org/abs/1703.09137), except the text "encoder" is a transformer encoder instead of an RNN, and the model is trained to predict the input text sequence shifted by 1 (like in a sequence to sequence model) rather than only the next character in the input sequence. The model is trained on Flikr8k. 

# Contents
The notebook flikr8k_all_descriptions is the "main" notebook. flikr8k_all_descriptions_cross_val.ipynb is a notebook I use for cross validation and testing other tweaks to preprocessing, etc.

# To do
I am currently testing models on Flickr30k, including a model that uses a pretrained ViT as an image encoder.
I may do more cross validation, but previously, it has been very time consuming with little relative improvements to performance.