---
title: Text Mining
emoji: 🔎
date: 2019-01-01T00:00:00.000Z
summary: "Exploring South Park Through Text Mining: A Data-Driven Analysis of
  Language, Emotion, and Dialogue"
metaDescription: "Exploring South Park Through Text Mining: A Data-Driven
  Analysis of Language, Emotion, and Dialogue"
tags:
  - NTLK
  - Spacy
  - Sumy
  - Python
  - ""
---
For this project, we dove into the world of South Park, analyzing the show’s dialogue to uncover patterns in language, sentiment, and character interactions. Leveraging a dataset from Kaggle with transcripts spanning 16 seasons, we processed, analyzed, and visualized key textual elements using tools like Python’s NLTK, spaCy, and WordCloud.

![South Park](/src/assets/img/sp.jpeg "South Park ")

Our analysis involved several steps, starting with sentiment analysis using VADER to assign polarity scores. This approach gave us insights into the general tone of each character's lines, revealing a notably positive tilt for characters like Mr. Garrison and Mr. Mackey. We then attempted character classification, using classifiers such as Naive Bayes, Decision Trees, and a fine-tuned DistilBERT model. While DistilBERT achieved the highest accuracy, the best-performing model still only classified character lines correctly 56% of the time, hinting at the complex nature of character-based language.

Finally, we experimented with text summarization, comparing extractive methods (Sumy summarizer) and abstractive techniques (Flan T5 model). Although extractive summaries provided coherent snapshots of dialogue, the T5 model offered more contextual summaries—despite challenges with continuity between batches of phrases. Through various NLP techniques, this project highlights the potential and limitations of automated analysis on multi-character, episodic data like South Park.