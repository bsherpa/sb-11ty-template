---
title: Big Data in GIS
emoji: 🌍
date: 2024-10-28T14:54:50.664Z
summary: Analyzing 30 Years of Temperature Trends in Piemonte
metaDescription: Analyzing 30 Years of Temperature Trends in Piemonte
tags:
  - python
  - pandas
  - xarray
  - NetCDF
  - geopandas
---
This project aimed to assess temperature trends in Piemonte over the past three decades by combining multiple data sources and GIS tools. We used data from ERA5 (Copernicus Climate Data) and ARPA Piemonte, with the ERA5 data in NetCDF format and ARPA data in CSV files. Using Python, i've handled data aggregation and manipulation with libraries like pandas for data handling, xarray for processing NetCDF files, and geopandas for integrating spatial data.

For visual exploration, i've employed Cartopy to create geographical plots, showcasing monthly temperature trends and anomalies. Statistical analysis, such as calculating correlation and regression models, was performed with statsmodels. Our findings revealed a consistent temperature rise, validated by high correlation between ERA5 and station data, underscoring the effectiveness of GIS and big data tools in environmental monitoring.