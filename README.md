# Quora-Insincere-Questions-Classification
![Screen Shot 2021-12-21 at 15 52 59](https://user-images.githubusercontent.com/41892953/147012273-2891fb99-79cc-4b7e-bc93-f35d841b38d9.png) 

## Problem Statement
An existential problem for any major website today is how to handle toxic and divisive content. [Quora](https://www.quora.com/) is a platform that empowers people to learn from each other. On Quora, people can ask questions and connect with others who contribute unique insights and quality answers. A key challenge is to weed out insincere questions -- those founded upon false premises, or that intend to make a statement rather than look for helpful answers. In this [kaggle competition](https://www.kaggle.com/c/quora-insincere-questions-classification), Kagglers will develop models that identify and flag insincere questions.

## Libraries
- scikit-learn
- Keras
- Tensorflow
- Numpy

## Files
- [`Quora_data_exploration.ipynb`](https://github.com/wmingch1992/Quora-Insincere-Questions-Classification/blob/main/Quora_data_exploration.ipynb) performs basic data exploration
![Screen Shot 2021-12-21 at 16 14 04](https://user-images.githubusercontent.com/41892953/147013797-ce733d88-f61a-4d18-ab56-6601e4731626.png)
- [`Quora_GRU_no_pretrain_embeddings.ipynb`](https://github.com/wmingch1992/Quora-Insincere-Questions-Classification/blob/main/Quora_GRU_no_pretrain_embeddings.ipynb) built [Gated Recurrent Unit](https://en.wikipedia.org/wiki/Gated_recurrent_unit)(GRU) neural network model without pretrained word embeddings to do the text classification
- [`Quora_GRU_with_pretrained_embeddings.ipynb`](https://github.com/wmingch1992/Quora-Insincere-Questions-Classification/blob/main/Quora_GRU_with_pretrained_embeddings.ipynb) built [Gated Recurrent Unit](https://en.wikipedia.org/wiki/Gated_recurrent_unit)(GRU) neural network model with pretrained word embeddings (i.e. [Glove]( https://nlp.stanford.edu/projects/glove/))


## Results 
- The evalution metric for this competiion is [F1 Score](https://en.wikipedia.org/wiki/F-score)
- The private score for GRU without pretrained word embeddings is 0.65286 (ranked 1242/4037, top 30.8%)
- The performance is improved with pretrained word embeddings (i.e., 0.67470, ranked 1182/4037, top 29%)

## Next step
- The results may be further improved by spell check
- use multiple pretrained word embeddings (including [GoogleNews](https://code.google.com/archive/p/word2vec/), [wiki-news-300d-1M](https://fasttext.cc/docs/en/english-vectors.html)), and make the classifications on top of multiple recurrent neural network models 
