# Social Media Sentiment Analysis with Google Cloud Natural Language API
This repository contains a project focused on analyzing the sentiment of social media tweets using the Google Cloud Natural Language API. The goal is to extract sentiment insights from tweets to understand public opinion trends and reactions on specific topics.

## Project Overview
### This project performs the following steps :

1. **Data Collection :** Twitter data collected, including various tweets for sentiment analysis.
2. **Data Cleaning :** The tweets are preprocessed to remove unnecessary text, links, special characters, etc.
3. **Language Detection :** Using the langdetect library, non-English tweets are filtered out with a try-except model to avoid unsupported languages in the API.
4. **Sentiment Analysis :** Google Cloud’s Natural Language API is used to determine the sentiment score and magnitude, identifying each tweet as Positive, Negative, or Neutral.
5. **Data Visualization :** The insights from sentiment analysis are visualized through pie charts, scatter plots, and histograms for a comprehensive understanding.

## Key Insights
+ ### Sentiment Distribution :
  + **Positive :** 47.8% (477 tweets)
  + **Negative :** 34.8% (347 tweets)
  + **Neutral :** 17.4% (174 tweets)
 
+ ### Visual Analysis :
  + **Pie Chart :** Displays overall sentiment distribution.
  + **Scatter Plot :** Shows sentiment scores across tweets, forming a "V" shape representing varying sentiment intensity.
  + **Histogram :** Illustrates the frequency distribution of sentiment scores, providing insight into the range of sentiment polarity.
 
## Libraries Used
+ `pandas` for data handling and manipulation
+ `re` for regular expression operations in text cleaning
+ `google-cloud-language` for accessing the Google Natural Language API
+ `langdetect` for detecting the language of each tweet
+ `matplotlib` for data visualization

## Usage
1. **Data Cleaning :**
    + Run the clean_tweet() function to preprocess and clean each tweet, removing unwanted characters, links, and whitespace.
2. **Language Detection and Sentiment Analysis :**
    + Execute the analyze_sentiment() function, which detects the language and performs sentiment analysis only if the tweet is in English.
    + This step outputs sentiment scores and magnitudes.
3. **Visualization :**
    + Use matplotlib to generate visualizations like pie charts, scatter plots, and histograms to analyze and interpret the sentiment data.

## Results
Through sentiment analysis, we identified a positive sentiment skew, with 47.8% of tweets showing positivity, while 34.8% were negative and 17.4% were neutral.
