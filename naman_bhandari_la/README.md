# Project 3 - Web APIs & Classification

For this project, I was learned how to use webscraping and Natural Language Processing (NLP) to train a classifier on which subreddit a given post came from. This was a binary classification problem.

I practiced the following skills in this project:

1. **Data wrangling/gathering/acquisition**

2. **Natural Language Processing** - converting standard text data (like Titles and Comments) into a format that allows us to analyze it and use it in modeling.

3. **Classification Modeling** 

### Prompt

Can we identify differences in language used by angry posters vs. depressed posters and build a model that can correctly predict depression in a person?

### Overview

Using some statistical tools such as TF-IDF Vectorizer and a Multinomial Naive Bayes model, as well as some API scraping tools, we are able to retrieve posts from two subreddits on Reddit.com and analyze them to build a model that can classify posts into the subreddits based on their semantic content.

I selected the r/rant and r/depression subreddits. Certain studies show that there is a link between anger and depression (see: https://psychcentral.com/blog/why-so-angry-irritable-it-might-be-depression/), so I thought it was useful to see if our model classified a post that is actually from r/rant as being from r/depression instead, which would indicate that the person who is "angry" may be exhibiting signs of depression.

### Materials

- Jupyter notebooks: 1-project-3_scrape.ipynb and 2-project-3_analysis.ipynb
- Presentation: Naman Bhandari - LA 5 - Project 3.pdf

### Technologies
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- CountVectorizer
- TfidfVectorizer
- MultinomialNB 

### Datasets

- r/depression JSON: ./data/depression.json
- r/rant JSON: ./data/rant.json

This data was scraped from Reddit using their API.