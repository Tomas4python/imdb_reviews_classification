# IMDB Sentiment Analysis with Keras

## Overview
This repository contains a Keras implementation for sentiment analysis on the IMDB movie review dataset. The goal is to classify movie reviews as positive or negative based on the text content.

## Models
The models are built using the Keras Sequential API with various architectures ranging from simple Dense networks to more complex structures involving Embeddings and LSTM layers.

## Repository Sructure
- ***keras_imdb_50_50.ipynb***: A Keras-based notebook for the classification task on the keras imdb dataset with original train/test (50%/50%) split - stable results 87-88% test accuracy.
- ***keras_imdb_85_15.ipynb***: A Keras-based notebook for the classification task on the keras imdb dataset with changed train/test (85%/15%) split -stable results 89% test accuracy.
- ***model_performance_metrics_imdb.xlsx***: An Excel file documenting the performance metrics of the keras imdb model.
  
## Results
Model experimentation led to the following insights:
- Simpler models tended to reach satisfactory performance quickly and effective.
- A balanced approach to growing of training and validation metrics equally during training provided stable and reliable results.
- Experimentation with hyperparameters and architectural modifications showed that a simpler model architecture with appropriate regularization achieved competitive scoring.
- Overly complex models or excessive regularization did not necessarily improve performance.
- Some claims of extremely high accuracies (>94%) on unseen data without pretrained embeddings found misleading (after testing provided code). Realistic test accuracy without pretrained embeddings on this dataset is around 88%.
