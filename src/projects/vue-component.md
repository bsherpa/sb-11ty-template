---
title: Deep learning - Guess film genre by movie poster and synopsis
emoji: 🎞️
date: 2019-01-01T00:00:00.000Z
summary: Deep learning - Guess film genre by movie poster and synopsis
metaDescription: Deep learning - Guess film genre by movie poster and synopsis
tags:
  - keras
  - python
  - bert
---
In this project, we developed a deep learning model capable of predicting a movie’s genre based on its synopsis and poster. Using **Keras** and a pre-trained **BERT** model, we combined text and image data to build a classifier that identifies genre from two distinct inputs, leveraging the powerful language understanding of **BERT** alongside visual insights.

Our approach started with text processing, where **BERT** was used to embed the movie synopsis into high-dimensional representations, capturing semantic nuances specific to each genre. For the visual component, we utilized convolutional neural networks (**CNNs**) in Keras to process movie posters, extracting key visual features. These text and image embeddings were then merged in a fully connected layer, allowing the model to learn associations between plot themes and visual style across genres.

The classifier underwent extensive training and evaluation, and we fine-tuned hyperparameters to improve accuracy. Testing showed that the model effectively captured genre-defining elements, especially in cases where synopses were rich in descriptive language or posters conveyed strong genre-specific visuals. This project highlights the versatility of combining text and image data in deep learning models, demonstrating how multimodal approaches can enhance predictive capabilities in applications like movie genre classification