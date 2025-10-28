# Zomato-Restaurant-Clustering-Sentiment-Analysis

# Problem Statement

With the increasing popularity of food delivery and online restaurant discovery platforms like Zomato, there is a massive amount of data available about customer reviews, restaurant types, cuisines, ratings, and costs. Understanding customer sentiment and grouping restaurants based on various characteristics can help both customers and business owners.

The objective of this project is to perform clustering of restaurants based on their features (like cuisines, cost, and popularity) and conduct sentiment analysis on user reviews to understand customer satisfaction levels.
The goal is to identify patterns in restaurant offerings and customer opinions, which can help improve business strategies and user experience.


# Data Description

The dataset is derived from Zomato and contains two major components:

# Restaurant Metadata (105 records)
Information about restaurant features and offerings.

Name: Restaurant name

Links: URL to restaurant’s Zomato page

Cost: Approximate cost for two people

Collections: Restaurant tags or themes (e.g., “Buffet”, “Hottest in Town”)

Cuisines: Types of cuisines served

Timings: Opening and closing hours

# Restaurant Reviews (10,000 records)
User feedback and experience details.

Restaurant: Restaurant name

Reviewer: User name

Review: Review text

Rating: User rating (1 to 5)

Metadata: User profile info (number of reviews/followers)

Time: Timestamp of review

Pictures: Number of images uploaded with review


# Data Exploration


Ratings Distribution:
The rating distribution is slightly skewed towards higher ratings (4–5), indicating that most customers share positive experiences.

Review Volume:
Certain restaurants like Paradise and Flechazo have significantly higher review counts, showing their popularity and high customer engagement.

Text Analysis:

Common positive words: “good”, “tasty”, “amazing”, “ambience”, “friendly”

Common negative words: “slow”, “bad”, “worst”, “overpriced”
This gives a quick overview of sentiment patterns.

Cuisines & Cost:
Restaurants serving multi-cuisine menus or premium categories tend to have higher average ratings.
The cost for two ranges roughly from ₹500 to ₹2,000.

Correlation Observation:
Higher-rated restaurants are more likely to appear in Zomato collections like “Hyderabad’s Hottest” or “Great Buffets”.
There is a moderate correlation between restaurant cost and average rating, suggesting that slightly costlier restaurants often provide better-rated experiences.

# Approach



Data Cleaning & Preprocessing

Merged the two datasets using the restaurant name.

Removed missing and duplicate entries.

Processed text reviews (tokenization, stopword removal, lemmatization).

Exploratory Data Analysis (EDA)

Analyzed rating trends, cost patterns, and cuisine distributions.

Visualized customer sentiments across cuisines and cost categories.

Sentiment Analysis

Applied VADER or TextBlob sentiment analysis on review texts.

Classified reviews as Positive, Neutral, or Negative.

Compared sentiment distribution with average rating.

Feature Engineering

Encoded categorical variables (Cuisines, Collections).

Normalized numeric features (Cost, Review Count, etc.).

Clustering

Used K-Means Clustering to group restaurants based on cost, rating, cuisines, and sentiment scores.

Optimal cluster count determined using the Elbow Method.

Model Evaluation & Visualization

Evaluated cluster compactness (Silhouette Score).

Visualized clusters using PCA or t-SNE for better interpretability.



# Learning Outcome



Gain hands-on experience in data cleaning, EDA, and feature extraction from textual data.

Understand how to perform sentiment analysis on customer reviews using NLP techniques.

Learn how to cluster entities (restaurants) based on multi-dimensional attributes.

Develop insights into how customer opinions and restaurant characteristics affect business strategies.

Strengthen understanding of unsupervised learning and text analytics concepts.
