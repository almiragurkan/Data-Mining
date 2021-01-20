# Data-Mining
DATA ANALYSIS OF AMAZON’S DATASET

Senem Yalın - Almira Gürkan

ABSTRACT

Data mining is the process of automatically discovering useful information in large
data repositories. We are drowning in data, but starving for knowledge. Natural language
processing (NLP) is an exciting branch of artificial intelligence (AI) that allows machines to
break down and understand human language. In this assignment, we used NLP techniques to
interpret text data that we are working with, for our analysis. In addition, Recommendation
System and Neural Network are used for prediction.

1-Introduction

This assignment has 7 steps which are Data Cleaning, Exploratory Data Analysis, Sentiment
Analysis, Text Generation, Regression, Neural Network Process, Recommendation Process. After
these steps, we had forward inferences.

2-Assignments

When we are doing text analysis part, we used several NLP libraries in Python including
TextBlob along with the standard machine learning libraries including pandas and scikit-learn.
We got results from the data which we analysed and plotted these results in many different ways.
Also we did Recommendation Analysis. After that, we printed the suggestions.

2.1 Data Pre-processing

2.1.1 Getting the data

We had 2 data sets, so we merged our data according to the columns that we will use. Our data
which we merged, has the columns below.
overall - rating of the product
reviewTime - time of the review (raw)
reviewerID - ID of the reviewer, e.g. A2SUAM1J3GNN3B
asin - ID of the product, e.g. 0000013714
reviewText - text of the review
title - name of the product
brand - brand name

2.1.2 Cleaning the data

We made text lowercase, removed punctuation and removed words containing numbers. Also
we got rid of some additional punctuation, non-sensical text that was missed the first time
around and stop words on ”reviewText” column.

2.1.3 Organizing the data

We organized the cleaned data into a way that is easy to input into other algorithms.

1-We assigned numbers to brands so that the machine could understand, and we gave the same
numbers to those with the same brand.

2.2 Brand Count

2.2.1 Exploratory Data Analysis

1-We grouped brands according to the number of products they sell.
2-We saw that how many products were purchased from which brand and how many brands
are there.
3-Because our data makes sense, we removed the most and least purchased brands from this
data.
4-We plotted our 2 results.

2.3 Comparing Analysis

2.3.1 Sentiment Analysis

1-We applied the ”sentiment.polarity” and ”sentiment.subjectivity” methods of the ”textblob”
library to find the polarity and subjectivity of brand’s ”reviewText”.
2-Each word in ”reviewText” column is labeled in terms of polarity and subjectivity.
3-We took the average subjectivity and polarity of product reviews that have the same brand
and assigned them to that brand.

Polarity: How positive or negative a word is. -1 is very negative. +1 is very positive.
Subjectivity: How subjective, or opinionated a word is. 0 is fact. +1 is very much an opinion.

4-We plotted these results
