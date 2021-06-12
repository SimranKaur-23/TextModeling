# TextModeling
NLP | Python
- This task was performed as a part of an academic assignment wherein the task was to  Perform Topic modeling on a social media corpus like Twitter or Reddit by using any python library. 
The topic modeling is done using LDA and NMF models.
## Datset
- the dataset can be accessed using [Dataset](https://github.com/SimranKaur-23/TextModeling/blob/main/climate_tweets.csv) or in the repository under the name climate.csv
## A gist of what i did...
 - Import the necessary libraries.
 - Read the dataset.
 - Used functions like info(), shape, describe(), unique() to know more about the dataframe.
 - The dataframe contains redundant tweets as well. This implies that our dataframe contains retweets.
 - So, next we add a separate column for retweets.
 - Used sum() on this column to find out that there are 773 retweets.
 - Using group by found out 10 most repeating tweets.
 - Plotted histogram of tweet counts.
 - Made new columns for retweeted usernames, mentioned usernames and hashtags.
 - Made a new dataframe hashtags_list_df which contains the rows from the hashtag columns where there are actually hashtags.
 - Created a dataframe flattened_hashtags_df where each use of hashtag gets its own row.
 - Made a new dataframe popular_hashtags which stores the count of appearances of each hashtag.
 - Plotted these popular hashtags using barplot.
 - Repeated similar steps (10 - 13) for mentioned usernames and retweeted usernames.
 - Made a new dataframe which checks columns to encode presence of hashtags.
 - Calculated the correlation matrix and plotted it using heatmap.
 - Defined a function to clean_tweet to clean the tweets from punctuations, usernames etc. and added a new column in the dataframe with the same name.
 - Used count vectorizer to transform text to vector form.
 - Used LDA model on the counter vectorized dataframe.
 - Made a function display_topics which displays the topic words and the corresponding word weights.
 - Used NMF model on the counter vectorized dataframe.
 - Used function display_topics to display the table.
