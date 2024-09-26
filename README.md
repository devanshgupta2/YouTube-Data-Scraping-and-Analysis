# YouTube Data Scraping and Analysis

## Introduction

This project involves scraping YouTube data using the **YouTube Data API**, analyzing the data with **Pandas**, and visualizing the results using **Seaborn**. The goal is to extract key statistics from YouTube channels and videos to gain insights into content performance and audience engagement.

## Project Overview

The project is split into two parts:

1. **Channel Statistics Extraction**:
   - We extract statistics like the number of subscribers, total views, and video counts for several YouTube channels.
   - The data is analyzed to compare channel performance and determine which channels have the highest engagement and reach.

2. **Video Details Extraction**:
   - This part involves extracting video-specific details such as video titles, views, likes, and comments.
   - These details are then analyzed to determine which videos perform the best in terms of engagement metrics.

## Steps to Build the Project

### 1. Setup YouTube Data API Key

To begin, you will need to create a YouTube Data API Key, which serves as the credential for accessing YouTube data. Follow [this link](https://console.cloud.google.com/) to generate your API key. The official documentation for using the API can be found on the [YouTube Data API documentation page](https://developers.google.com/youtube/v3).

### 2. Set Up Jupyter Notebook

Since this project is built using Jupyter Notebook, ensure you have Jupyter installed. You can install it using the following command if needed:

```bash
pip install notebook
```
```bash
!pip install google-api-python-client pandas seaborn
```

### 3. Scrape YouTube Data

Using the YouTube Data API, the project scrapes data related to:

- **Channel Statistics**: Information such as channel name, subscriber count, total views, and total number of videos.
  
- **Video Details**: Information about each video on a channel, including the title, number of views, likes, comments, and dislikes.

### 4. Data Analysis

The collected data is then loaded into Pandas DataFrames for further analysis. We examine various metrics to determine which channels have the highest performance and analyze video engagement patterns.

### 5. Data Visualization

Finally, using the Seaborn library, we generate visualizations to better understand and compare the extracted data. Visuals include bar plots of subscriber counts, total views, and video statistics, making it easier to spot trends and insights.

## Libraries Used

- **google-api-python-client**: For accessing YouTube Data API and fetching YouTube channel and video data.
- **pandas**: To organize and analyze the data.
- **seaborn**: To create data visualizations that help highlight key insights.

## Insights Gained

After scraping and analyzing YouTube data, several interesting insights were discovered:

1. **Channel Performance**:
   - Channels with higher subscriber counts may not always have the highest view counts, suggesting that some channels attract niche but highly engaged audiences.
   - The frequency of video uploads doesn't necessarily correlate with higher views—quality over quantity seems to play a role in audience engagement.

2. **Video Engagement**:
   - Videos that receive more views generally also receive higher numbers of likes and comments, showing a positive correlation between visibility and engagement.
   - Certain video topics or formats tend to attract more audience interaction, which can help guide content strategies for channel growth.

## Conclusion

This project successfully demonstrates how to scrape and analyze YouTube data using Python. By analyzing and visualizing the data, we can gain valuable insights into the performance of YouTube channels and videos, allowing content creators to refine their strategies and better understand their audience. The use of Pandas for data analysis and Seaborn for visualizations makes the data easy to interpret and actionable for decision-making.

