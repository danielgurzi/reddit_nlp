
### Contents:
- [Executive Summary](#Executive-Summary)
- [Problem Statement](#Problem-Statement)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)
- [About the Data](#About-the-Data)
- [Data Dictionary](#Data-Dictionary)

### Executive Summary
Looking for investment advice? The top two subreddits for beginning investors are r/investing and r/personalfinance according to https://www.makeuseof.com/tag/10-best-subreddits-finance/. R/personalfinance is geared more toward beginning investors, or those who are looking for how to better manage their money, where r/investing is still general, but focusing more on the market than on more general financing topics like credit cards and savings accounts. 

### Problem Statement 

We have just taken control of our financials and are wanting to make sure we have built a good foundation, but we also want to start trading stocks and exploring the market. Having successfully rebuilt our financial foundation from r/personalfinance, let's make sure we know which piece of advice is coming from which subreddit to know what level of caution or confidence we can have with the new post. 


### Conclusions and Recommendations

We can predict with 87% accuracy which subreddit the post is coming from and can therefore apply that level of confidence in following the advice of the subreddit whether it be from r/personalfinance or r/investing


### About the Data

I utilized Pushshift's API to bring in posts from 2 different reddits. I was able to pull 500 posts at a time from each subreddit and then appended them into a single dataframe and saved it as a csv to import and utilize in the modeling python sheet. 

I have sorted the data into this top directory and a folder to hold csvs. 
|__ README.md
   |__ you are here
|__ Invest-It_w_Reddit-DanielGurzi-GA_Project-3.pdf
|__ data_pull.ipnyb
   |__ pythong workbook for pulling subreddit posts
|__ data_processing.ipynb
   |__ python workbook for modelling data
|__ /datasets
   |__ csv files
|__ /images
   |__ support images for presentation 


### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|r/personalfinance|      url | www.reddit.com/ | The url suffix location on Reddit for the first subreddit | 
|r/investing      |      url | www.reddit.com/ | The url suffix location on Reddit for the first subreddit | 
|subreddit        |   object | data.csv        | The column holding the name of the subreddit
|selftext         |   object | data.csv        | The text of the post on the subreddit | 
|title            |   object | data.csv        | The title of the post on the subreddit | 
