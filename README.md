# Exploratory Data Analysis: Instagram Dataset
This project analyzes Instagram post data to uncover insights into post performance, engagement, and reach. Using Python and data visualization libraries, we explore key metrics such as likes, comments, shares, impressions, and follower growth. The goal is to identify trends, optimize content strategy, and improve overall engagement.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Tools and Libraries](#tools-and-libraries)
4. [Key Analyses](#key-analyses)
5. [Steps Taken](#steps-taken)
6. [Visualizations](#visualizations)
7. [Key Insights](#key-insights)
8. [Constraints](#constraints)
9. [Future Work](#future-work)
10. [Contact](#contact)

---

## Project Overview
This project focuses on analyzing Instagram post data to answer questions such as:
- Which posts have the highest engagement?
- Which sources contribute the most to impressions?
- How do hashtags impact post performance?
- What is the relationship between profile visits and new followers?

The analysis is performed using Python, with visualizations created using Plotly, Seaborn and Matplotlib. The results are presented in interactive charts and graphs.

---

## Dataset Description
The [dataset](https://github.com/tamunoWoks/Exploratory_Data_Analysis_Instagram_Dataset/blob/main/Instagram_data.csv) used was gotten from [Statso.io](https://statso.io/instagram-reach-analysis-case-study/).  

The dataset contains the following columns:
- **Impressions**: Total number of times the post was seen.
- **From Home**: Impressions from the user's home feed.
- **From Hashtags**: Impressions from hashtags.
- **From Explore**: Impressions from the Explore page.
- **From Other**: Impressions from other sources.
- **Saves**: Number of times the post was saved.
- **Comments**: Number of comments on the post.
- **Shares**: Number of times the post was shared.
- **Likes**: Number of likes on the post.
- **Profile Visits**: Number of profile visits from the post.
- **Follows**: Number of new followers gained from the post.
- **Caption**: The caption of the post.
- **Hashtags**: Hashtags used in the post.

---

## Tools and Libraries
- **Python**: Primary programming language.
- **Pandas**: Data manipulation and analysis.
- **Plotly**: Interactive data visualizations.
- **Matplotlib**: Static data visualizations.
- **Seaborn**: Statistical data visualization.
- **TextBlob**: Sentiment analysis.

---

## Key Analyses
1. **Engagement Analysis**:
   - Identify posts with the highest engagement (likes, comments, shares).
   - Calculate the engagement rate for each post.

2. **Source Analysis**:
   - Determine which source (home, hashtags, explore, other) contributes the most to impressions.

3. **Hashtag Performance**:
   - Analyze the impact of hashtags on engagement and impressions.

4. **Follower Growth**:
   - Track follower growth over time and identify posts that drive the most follows.

5. **Correlation Analysis**:
   - Explore relationships between metrics like impressions, likes, comments, and shares.

6. **Sentiment Analysis**:
   - Analyze the sentiment of post captions (positive, negative, neutral).

---

## Steps taken:
- Import necessary libraries.
- Load and overview data
    - The encoding='latin1' parameter in the pd.read_csv() function specifies the character encoding used to read the CSV file.
    - Use it when your CSV file contains characters that are not supported by the default UTF-8 encoding.
    - Use it if you encounter a UnicodeDecodeError while reading the file.
- View column info of dataset
- View descriptive statistics of dataset
- Check data for inconsistencies (null values)
- Create a histogram for the 'Impressions' column
- Create a line plot showing trend of impressions over time.
    - The dataset doesn’t explicitly have a time-based column (e.g., a date or timestamp).
    - Hence I used the row index (data.index) as the x-axis.
    - In other use cases, this might not be meaningful unless the rows are ordered chronologically.
- Create a multi-line plot that shows the trends of Likes, Saves, and Follows over time.
    - Once again, I use the row index (data.index) as the x-axis.
- Create a pie chart that visualizes the distribution of reach (impressions) from different sources: From Home, From Hashtags, From Explore, and From Other.
- Create a pie chart that visualizes the distribution of engagement metrics: Saves, Comments, Shares, and Likes.
- Create a scatter plot with a trendline to visualize the relationship between Profile Visits and Follows.
- Create a word cloud for the hashtags used in the Instagram posts.
    - plotly.express (px) does not directly support creating word clouds. 
    - The WordCloud library from wordcloud can be used to generate the word cloud and then display it using matplotlib.
- Create a correlation matrix heatmap to visualize the relationships (correlations) between different numerical features in your dataset.
- Create a correlation matrix heatmap to xplore the relationships between different metrics (e.g., impressions, likes, comments, shares) to identify patterns.
- Create a bar chart that visualizes the distribution of the top 25 hashtags used in the Instagram posts.
- Create two bar charts to visualize the distribution of top 25 Likes and Impressions for each hashtag used.
- Create a histogram to to analyze the sentiment of the captions (positive, negative, neutral), with the sentiment analysis library TextBlob.
- Use a scatterplot to analyze the relationship between profile visits and new followers to understand how effectively profile visits convert into followers.
- Use a scatterplot to analyze how the length of your captions (number of words or characters) affects engagement.

---

## Visualizations
Here are some of the visualizations created in this project:

1. **Top 10 Posts by Engagement**:
   ![Top 10 Posts by Engagement](images/top_engagement.png)

2. **Contribution of Sources to Impressions**:
   ![Source Contribution](images/source_contribution.png)

3. **Hashtag Performance**:
   ![Hashtag Performance](images/hashtag_performance.png)

4. **Engagement Rate Analysis**:
   ![Engagement Rate](images/engagement_rate.png)

---

## Key Insights
1. **Engagement**:
   - Posts with more likes tend to have higher comments and shares.
   - The top 10 posts account for 40% of total engagement.

2. **Impressions**:
   - The majority of impressions come from the home feed, followed by hashtags and the Explore page.

3. **Hashtags**:
   - Posts with popular hashtags like `#datascience` and `#python` receive higher engagement.

4. **Follower Growth**:
   - Posts with high profile visits tend to drive more new followers.

5. **Sentiment**:
   - Captions with positive sentiment tend to perform better in terms of engagement.

---

## Constraints
- Captions were too long, so it was not impossible to make visalizations about them.
- There was no timestamp or date column, therefore we were limited and couldn't make Time-based analysis

--- 

## Future Work
- Incorporate machine learning models to predict post performance.
- Analyze the impact of posting time on engagement.
- Expand the dataset to include more metrics (e.g., video views, story interactions).
- Build an interactive dashboard using Dash or Streamlit.

--- 

## Contact
For questions or feedback, feel free to reach out:

Name: [Your Name]

Email: [Your Email]

GitHub: [Your GitHub Profile]

LinkedIn: [Your LinkedIn Profile]


