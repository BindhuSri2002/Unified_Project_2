# Unified_Project_2

# Project Description
This notebook is focused on analyzing climate-related text data from NASA’s social media posts. It combines data preprocessing, text analysis, sentiment analysis, and visualization to extract meaningful insights.

# 1. Libraries Used

The following libraries are used throughout the notebook:

pandas → for loading the dataset, cleaning data, and performing analysis.

matplotlib & seaborn → for creating bar charts, histograms, and trend plots.

wordcloud → to generate word cloud visualizations from text.

nltk (Natural Language Toolkit) → for text analysis and sentiment scoring.

SentimentIntensityAnalyzer (from NLTK) → for VADER sentiment analysis.

# 2. Data Loading and Cleaning

The dataset (climate_nasa.csv) is loaded into a DataFrame.

The date column is converted into proper datetime format.

Missing values are checked. Missing text entries are replaced with empty strings to avoid errors in analysis.

# 3. Engagement Metric

A new column engagement is created as the sum of likes and comments.

Profiles are grouped by their names to calculate total engagement.

A bar chart is used to highlight the top 10 most engaging profiles.

# 4. Word Cloud (Common Words)

All the text data is combined into one large document.

A word cloud is generated to visualize the most frequently used words.

This highlights the most common topics/themes in climate-related discussions.

# 5. Sentiment Analysis

The VADER lexicon is downloaded (a pre-trained sentiment dictionary).

Each text entry is given a sentiment score:

Positive (> 0)

Negative (< 0)

Neutral (~0)

A histogram shows how sentiment is distributed across all posts.

# 6. Sentiment by Profile

The average sentiment score is calculated for each profile.

The top 10 profiles with the most positive sentiment are identified.

Results are visualized with a bar chart.

# 7. Time-Series Sentiment Trend

Sentiment scores are grouped by month.

A time-series line plot is created to track how average sentiment changes over time.

This helps identify whether climate discussions became more positive, negative, or neutral in different periods.
