# Youtube Video Performance

## Project Overview
### Introduction
YouTube is one of the largest and most popular platforms globally, with billions of searches and active users every month. For content creators, especially in niches like travel, understanding the key drivers of views and engagement is crucial. This project explores the relationship between various video metrics and view counts by analyzing data from the 10 most popular YouTube travel channels.

The project involves Exploratory Data Analysis (EDA) and statistical testing to provide insights into how different factors, such as likes, comments, video duration, and captions, influence video performance.

## Objectives
The project aims to:

* Explore the YouTube API to extract video data.
* Analyze video data to answer the following questions:
  * Does the number of likes or comments impact the number of views a video gets?
  * Does video duration influence views or interaction (likes/comments)?
  * Does title length affect video views?
  * How many tags do high-performing videos have? What are the common tags?
  * How frequently do the top travel content creators upload videos? Which days of the week have the most views?
* Perform two-sample t-tests to determine if having captions influences video views.
* Apply NLP techniques to uncover:
  * Popular topics covered in the videos (e.g., word clouds from video titles).
### Data
For this project, I created a custom dataset by using the YouTube API. The dataset contains information about 10 famous travel YouTube channels:

* The Endless Adventure
* Abroad in Japan
* Drew Binsky
* Hey Nadine
* Wolters World
* Adventures of A+K
* Flying The Nest
* Kara and Nate
* Indigo Traveller
* FunForLouis
## Data Creation with YouTube API
Steps to Acquire the Data:
* Google Developers Console: Created a project and requested API access credentials.
* API Key: Generated an API key to send requests to the YouTube API.
* YouTube API Enablement: Enabled the YouTube Data API to fetch video and channel statistics.
* Channel IDs: Obtained channel IDs by inspecting each channel's information on YouTube.
* API Functions: Wrote custom functions to collect channel statistics and video-level data.
## Key Findings and Insights
The analysis revealed several key insights regarding the performance of videos on YouTube travel channels:

* There is no clear correlation between the number of comments per 1000 views or likes per 1000 views and overall view counts.
* Most travel videos are shorter than 1000 seconds (~16 minutes).
* Shorter videos tend to get more likes and comments than longer videos.
* Most-viewed videos tend to have a title length between 25-50 characters. Titles that are too short or too long seem to negatively impact viewership.
* The most-viewed videos generally have fewer than 35 tags.
* There is no clear pattern in video upload frequency by day of the week, but weekend videos tend to get more views than weekday videos.
* Videos with captions receive significantly more views compared to those without captions, as revealed by a statistically significant t-test.
## Limitations and Future Considerations
### Project Limitations:
* The dataset is relatively small, with data from around 10,700 videos.
* Comment data was not included due to YouTube API quota limits.
* Other influential factors, such as marketing efforts, government censorship, or YouTube’s recommendation algorithm, were not considered.
### Future Considerations:
* Expand the dataset to include more channels in the travel niche.
* Include comment data and perform sentiment analysis to understand which videos attract more positive or negative reactions.
* Conduct similar research for other content niches, such as beauty, language learning, or technology, and compare patterns in viewership and video characteristics across different niches.
