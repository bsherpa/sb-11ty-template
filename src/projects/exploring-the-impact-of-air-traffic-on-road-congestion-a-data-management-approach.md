---
title: "Exploring the Impact of Air Traffic on Road Congestion: A Data
  Management Approach"
emoji: ✈️
date: 2024-10-27T18:06:08.429Z
summary: A Data Management Approach to air traffic and road congestion
tags:
  - KNIME
  - python
  - MongoDB
  - Raspberry
---
This project aimed to analyze the relationship between air traffic at major Italian airports and the associated road traffic around these areas. We focused on four airports—Bergamo, Rome, Naples, and Catania—and collected data over 26 days using Google and TomTom APIs to monitor road traffic and custom web scraping techniques to track flight data.

Data was stored and managed in MongoDB, where we merged traffic and flight data based on timestamps, aligning road traffic volume with flight schedules. Using KNIME for preprocessing, we filtered, cleaned, and aggregated the data, establishing a comprehensive dataset for each airport. Our analysis considered data completeness, accuracy, and consistency, implementing time-based rules to associate flights with traffic measurements within relevant intervals.

Although initial results showed minimal correlation, the project demonstrated robust data management techniques and set the stage for future research, such as analyzing traffic patterns on different routes or examining peak hours for flights and road congestion.