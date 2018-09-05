# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)
#### About the API

Reddit's API is fairly straightforward. For example, if I want the posts from [`/r/boardgames`](https://www.reddit.com/r/boardgames), all I have to do is add `.json` to the end of the url: https://www.reddit.com/r/boardgames.json

To help you get started, we have a primer video on how to use Reddit's API: https://www.youtube.com/watch?v=5Y3ZE26Ciuk

---

### Objectives

- Scrape and prepare your data using the `requests` library.

**Pro Tip 2:** Reddit will give you 25 posts **per request**. To get enough data, you'll need to hit Reddit's API **repeatedly** (most likely in a `for` loop). _Be sure to use the `time.sleep()` function at the end of your loop to allow for a break in between requests. **THIS IS CRUCIAL**_

**Pro tip 3:** The API will cap you at 1,000 posts for each subreddit (assuming the subreddit has that many posts).

**Pro tip 4:** At the end of each loop, be sure to save the results from your scrape as a `csv`: JSON from Reddit > Pandas DataFrame > CSV. That way, if something goes wrong in your loop, you won't lose all your data.

---
This project covers three import concepts: Data Wrangling/Acquisition, Natural Language Processing, and Classification Modeling.

Data Wrangling/Acquisition-
Not all the data is in clean CSVs or a single table in SQL. Part of the code scrapes unstructured and semi-structures sources from Reddit.


This project focuses on **Natural Language Processing** by converting standard text data (like Titles and Comments) into a format that allows us to analyze it and use it in modeling.

This project also focuses on **Classification Modeling**.  That is, how do we determine what each Reddit post should be categorized as. For the objective of this lab, I want to find all the reddit posts that should be placed in the nba subreddit. I have introduced several categories of data to see how accurately the model can classify the right reddit posts as nba subreddit.  
