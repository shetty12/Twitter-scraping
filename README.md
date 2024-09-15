
# Twitter Data Scraping Bot

This project implements a Twitter bot that scrapes tweets from a specific Twitter account using the Tweepy API. The scraped data is processed and stored in a database for analysis using SQL queries.

About the Project

Project Overview
The bot fetches recent tweets from a specified Twitter user and extracts important information like tweet ID, creation date, number of likes, source of the tweet, language, location, retweet count, and tweet entities. It also scrapes tweets containing specific hashtags or keywords. The data is then saved in a CSV file and imported into an SQLite database. SQL queries are used to perform various analyses such as identifying the tweet with the most likes, the least likes, and tweet distribution based on the date or keyword.

Objectives
Data Collection: Extract data from Twitter using the Tweepy API.
Data Storage: Save the scraped data into CSV and SQLite database.
Data Analysis: Perform queries to analyze the most liked tweets, tweet sources, and other patterns.
Insights: Understand trends such as the distribution of tweets over time, source of tweets, and user interaction.
Technology Stack
Python: Used for building the bot, handling API calls, and data manipulation.
Tweepy: Twitter API wrapper to fetch tweets.
SQLite: Database for storing and querying the scraped tweets.
Pandas: For data manipulation and cleaning.
Regex: Used to extract and filter tweets based on hashtags or keywords.
Key Features
Twitter Scraping:

Scrapes recent tweets from a specified account.
Pulls data such as tweet ID, creation date, number of likes, source, and retweet count.
Scrapes tweets based on specific keywords or hashtags.
Data Storage:

Saves the scraped data in a CSV file.
Stores the data in an SQLite database for easy querying and analysis.
SQL Queries:

Analyze the tweet with the most and least likes.
Group and count tweets based on source, date, or keyword.
Query tweets within a specific date range or containing specific keywords.
Data Model
Twitter Data:
Tweet ID
Creation date
Number of likes
Tweet text
Source of tweet
Language
Location
Retweet count
Entities (hashtags, mentions)
Example Queries
Most Liked Tweet: Query the tweet with the maximum number of likes.
Least Liked Tweet: Query the tweet with the minimum number of likes.
Tweets within Date Range: Filter tweets based on creation date.
Tweets by Keyword: Search for tweets that mention specific keywords (e.g., "job").

Usage
Scraping Tweets: The bot can scrape tweets based on a username and a specific number of tweets. You can modify the username and the number of tweets directly in the script.

Data Analysis: Run SQL queries to analyze the scraped data. Example queries are provided in the script.

Export Data: The scraped tweets are exported to a CSV file for further analysis.

## Badges



[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
![Python](https://img.shields.io/badge/python-3.8-blue.svg)
![Pandas](https://img.shields.io/badge/pandas-1.2.4-blue.svg)
![NumPy](https://img.shields.io/badge/numpy-1.19.2-orange.svg)
![Matplotlib](https://img.shields.io/badge/matplotlib-3.3.4-orange.svg)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-0.24.2-yellow.svg)
![Scipy](https://img.shields.io/badge/scipy-1.6.0-lightgrey.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-brightgreen.svg)
![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Mac%20%7C%20Linux-blue)


## Deployment

To deploy this project run

```bash
  npm run deploy
```
Navigate to the directory and install the required libraries:
```bash
pip install tweepy pandas sqlite3
```
Create a Twitter Developer Account and get your API keys
```bash
 consumer_key = "your_consumer_key"
consumer_secret = "your_consumer_secret"
access_token = "your_access_token"
access_token_secret = "your_access_token_secret"
```

Run the script:
```bash
python twitter_scraper.py
```






