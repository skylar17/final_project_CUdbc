![Array of Women's Clothes](./Images/Womens_Clothes)

# Women's Clothing E-Commerce Data Analysis

#### Columbia University Data Analytics Bootcamp - Final Project (October 2020) 
#### Project By: Alfonso Toruno, Chris Campell, Himani Manglik, Kamal Mukherjee, Shivani Thakkar
--------------------------------------------------------------------------------------------------
## Goal
#### Visualize trends based on women's clothing e-commerce reviews and find a machine learning model that can most accurately predict consumer sentiment.

## Introduction
Our dataset came from Kaggle and is a collection of women’s clothing e-commerce reviews, written by prospective buyers and actual customers. All references to retailers have been anonymized. The raw columns are:

* Clothing ID
* Reviewer Age
* Review Title
* Review Text
* Rating
* Recommended (binary values)
* Positive Feedback Count
* Division Name
* Department Name
* Class Name

![Data Process](./Images/data_cleaning)

## Methods
For the <ins>ETL process</ins>, we performed a raw data cleanse, which included replacing null values with mode values, transposing the dataframe, and calculating the polarity and sentiment score. 
To make our data visualizations, we used <ins>Plotly, PIL</ins>, <ins>Matplotlib, Seaborn</ins>, and <ins>Python, Pandas</ins>. Some of the visualizations included bar charts, pie chart, 3-D chart, and heatmaps. We also made Word Cloud's for positive titles, negative titles, and review text. 

For the Machine Learning Analysis, we used toolkits like <ins>Wordcloud</ins>, <ins>NLTK</ins>, and <ins>SciKit-Learn (SkLearn)</ins>. For the ML Analysis Benchmark, we dropped stop words, tokenize & lemmatized, identified positive and negative words, and processed TD-IDF Matrix. Then, we trained, tested and predicted the accuracy of five models:

* Logistic Regression
* Support Vector Machines
* Naive Bayes
* Random Forest
* Neural Network

The highest accuracy score was taken by logistic regression and the lowest by neural network.

## Findings

Some of our findings include: 

1. Millennials proved to be the most outspoken with their product reviews, followed by the Generation X. 
2. The majority of the reviews in this dataset are incredibly positive (4 & 5), and we see that same trend across all age groups.
3. Consumers left the most reviews about categories like Tops, Dresses and Knits, while leaving far fewer about sleepwear, swimwear, casual bottoms etc.
4. Our Sentiment Analysis demonstrates that the consumers usually have a strong sentiment one way or the other and for this dataset, less than 25% of the reviewers expressed a neutral sentiment. 
5. While our dataset does not provide any information on actual sales conversions, by looking at other consumer behavior datasets we can confidently assume that customers with positive sentiment are likely to make (or have made) an actual purchase.
6. We have also processed our dataset through five different machine learning models to project consumer’s sentiment based on their review text. For our dataset Logistic Regression was the most accurate model and Neural Network was the least.








