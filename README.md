# INSTAGRAM REACH ANALYSIS
Python EDA project using instagram data 

Below are all the features in the data:
1. Impressions: Number of impressions in a post (Reach)
2. From Home: Reach from home
3. From Hashtags: Reach from Hashtags
4. From Explore: Reach from Explore
5. From Other: Reach from other sources
6. Saves: Number of saves
7. Comments: Number of comments
8. Shares: Number of shares
9. Likes: Number of Likes
10. Profile Visits: Numer of profile visits from the post
11. Follows: Number of Follows from the post
12. Caption: Caption of the post
13. Hashtags: Hashtags used in the post

Steps taken:
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
