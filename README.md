# Alcohol-Related Content on Social Media
The code and data in this repository is an example of a reproducible research workflow for MACS 30200 "Perspectives on Computational Research" at the University of Chicago./
The code is written in Python 3.9.7 and all of its dependencies can be installed by running the following in the terminal (with the `requirements.txt` file included in this repository):
```
pip install -r requirements.txt
```
## **Alcohol-Related Content on Twitter**
Codes in `Scraping_Twitter.ipynb` can be used to scrape tweets that is tagged with `#alcohol`.
You can then run codes in the jupyter notebook `Analysis_Twitter.ipynb` to replicate results in the final paper.
### Most frequent words associated with #alcohol
```
#deal, #alcohol, #gifts, #travel, #business, #marketing, #shopping, #affiliate, #affiliatemarketing, #blogger, #discount, #socialmedia, #twitter, #Beer, #drinks, #wine, #liquor, #deals, #ad, #affiliated
```
<img width="398" alt="image" src="https://user-images.githubusercontent.com/91500767/165214541-0212f944-79d5-482e-a8a9-6cbdf165a7b1.png">
<img width="341" alt="image" src="https://user-images.githubusercontent.com/91500767/165214568-07da0713-af60-45cb-990e-7f0eb0cc7164.png">

### Sentiment Analysis
Positive, Negative, Neutral and Compound Sentiment Scores
```
The mean positive sentiment score: 0.034672972385301155
The mean negative sentiment score: 0.023756468797564666
The mena neutral sentiment score: 0.9415688193085456
The mean compound sentiment score: 0.026897195042400485
```
## **Alcohol-Related Content on Reddit**
Search results on `reddit.com` yields subreddits most relevant to alcohol. Codes in `Scraping_Reddit.ipynb` can be used to scrape submissions and comments within those subreddit communities.
You can then run codes in the jupyter notebook `Analysis_Reddit.ipynb` to replicate results in the final paper.
```
ANALYSES ONGOING
```
