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
- [`Expedia_learning_to_rank_with_parameter_tuning.ipynb`](https://github.com/wmingch1992/Expedia-Learning-to-rank/blob/main/Expedia_learning_to_rank_with_parameter_tuning.ipynb) built a machine learning-to-rank model using [XGBoost](https://xgboost.readthedocs.io/en/stable/).

## Results 
- The evalution metric for this competiion is [Normzlied Discounted Cumulative Gain](https://towardsdatascience.com/normalized-discounted-cumulative-gain-37e6f75090e9) (NDCG@38) 
- The private score is 0.50340 (ranked 49/336, top 14.6%)

## Next step
- The results could be further improved by tuning the XGBoost hyperparameters 
- train a meta-model on top of XGBoost, lightGBM and Catboot learning to rank models
