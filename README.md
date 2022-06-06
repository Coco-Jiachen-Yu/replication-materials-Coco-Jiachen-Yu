# Alcohol-Related Content on Social Media
Yu, C. (2022). MACS 30200 Final Project (Version 1.0.0) [Computer software]

**Project Descriptions:**

**Individuals’ alcohol use is heavily influenced by emotional and social context, and previous studies have pinpointed socio-emotional factors as predictors for problematic drinking. With the insurgence of social media, a new virtual social environment has been constructed where individuals can share and discuss alcohol-related posts. However, there is a dearth in large-scale research that examine alcohol content on social media outside the laboratory context. As studies have revealed that exposure to alcohol-related cues can incentivize people to drink and even lead to hazardous drinking, it is important to know that nature of alcohol-related posts online. Realizing this interest and gap, the current study is aimed at exploring: 1) what topics are mostly discussed; and 2) what are the intrinsic sentiments embedded in the text, especially for the different topical communities. State of the art research tookits—a graphical network approach using Infranodus and sentiment analysis via the NLTK Vadar package—was utilized for content analysis. To achieve the research goal, this study pooled 369,386 tweets with keyword alcohol in April 2022, and 21 subreddit communities via Snscrape. For each subreddit community, 5,000 posts were scraped. The final sample size for each subreddit ranged from n = 22 to n = 4,462. Several salient topical clusters were identified, including health and fitness, addiction and time related words (e.g., years) on both platforms, other substances on Twitter and subjective feelings on Reddit. A lack of alcohol marketing on both platforms was detected, probably due to methodological constraints. Findings indicate that there is an overall higher positive sentiment compared to negative sentiment on both social media platforms. However, Twitter’s composite sentiment score leaned towards neutral. Regression analysis indicated that different subreddit communities have different sentiment scores across all valences. Aggregated data also revealed that posts featuring social drinking activities presented the highest positive sentiment score. Nonetheless, alcohol abstinence communities also demonstrated the highest compound score, thus an overall positive sentiment in their texts. Findings in this study provide important implications that alcohol presents a positive image online and serve as a warning sign that they might promote hazardous drinking. However, the overall positive environment on Reddit alcohol abstinence communities created a positive environment that might helpfully motivate people to restrain from alcohol use. Several imitations should be noted that methodological confined the study’s ability to directly test individuals’ drinking behaviors. New methodological approaches should be adopted to identify alcohol marketing content on social media platforms. Future research should also expand on exploring the social elements embedded in the texts and tested category-level sentiment scores for Twitter as well.**


The code and data in this repository is an example of a reproducible research workflow for MACS 30200 "Perspectives on Computational Research" at the University of Chicago.

The code is written in Python 3.9.7 and all of its dependencies can be installed by running the following in the terminal (with the `requirements.txt` file included in this repository):
```
$ pip install -r requirements.txt
```

## 1. Data Scraping
Enter the following commands in the terminal
```
$ snscrape --jsonl --max-results 5000 reddit-subreddit stopdrinking >reddit-@stopdrinking
$ snscrape --jsonl --max-results 5000 reddit-subreddit cripplingalcoholism >reddit-@cripplingalcoholism
$ snscrape --jsonl --max-results 5000 reddit-subreddit drugscirclejerk >reddit-@drugscirclejerk
$ snscrape --jsonl --max-results 5000 reddit-subreddit Drugs >reddit-@Drugs
$ snscrape --jsonl --max-results 5000 reddit-subreddit beer >reddit-@beer
$ snscrape --jsonl --max-results 5000 reddit-subreddit drunk >reddit-@drunk
$ snscrape --jsonl --max-results 5000 reddit-subreddit Alcoholism_Medication >reddit-@Alcoholism_Medication
$ snscrape --jsonl --max-results 5000 reddit-subreddit dryalcoholics >reddit-@dryalcoholics
$ snscrape --jsonl --max-results 5000 reddit-subreddit AlcoholGifRecipes >reddit-@AlcoholGifRecipes
$ snscrape --jsonl --max-results 5000 reddit-subreddit alcoholism >reddit-@alcoholism
$ snscrape --jsonl --max-results 5000 reddit-subreddit alcoholicsanonymous >reddit-@alcoholicsanonymous
$ snscrape --jsonl --max-results 5000 reddit-subreddit Sober >reddit-@Sober
$ snscrape --jsonl --max-results 5000 reddit-subreddit AlAnon >reddit-@AlAnon
$ snscrape --jsonl --max-results 5000 reddit-subreddit trees >reddit-@trees
$ snscrape --jsonl --max-results 5000 reddit-subreddit Marijuana >reddit-@Marijuana
$ snscrape --jsonl --max-results 5000 reddit-subreddit kratom >reddit-@kratom
$ snscrape --jsonl --max-results 5000 reddit-subreddit alcoholic >reddit-@alcoholic
$ snscrape --jsonl --max-results 5000 reddit-subreddit alcoholabuse >reddit-@alcoholabuse
$ snscrape --jsonl --max-results 5000 reddit-subreddit alcoholfreebeer >reddit-@alcoholfreebeer
$ snscrape --jsonl --max-results 5000 reddit-subreddit alcoholismprotips >reddit-@alcoholismprotips

$ snscrape --jsonl twitter-search 'alcohol since:2022-04-01 until:2022-05-01' >twitter-@alcohol.json
```

## 2. Network Analysis on Infranodus
### Graphical Visualization

<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/172096852-797b1ba1-34c0-4e58-9ac5-ea9b4c03b8e7.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/172096860-3bf22bca-62d2-4a04-b7a2-cf9be04ab212.png">

### Topic Modeling

![image](https://user-images.githubusercontent.com/91500767/172096967-76115ffa-1e39-4748-bd9b-968ed8d08466.png)
![image](https://user-images.githubusercontent.com/91500767/172097060-0bd72f92-b3e7-4c3a-9bee-900cc0bb04fc.png)

**Betweenness Centrality**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/172097111-5c593251-b084-4378-91c5-4c710c31f9a6.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/172097119-b12cef62-7f37-4688-9a94-47c54a17baa7.png">

**Degree and Frequency for Most Influential Words**

<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/172097156-a7fcc128-19aa-4421-b425-107e1ea98dc2.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/172097165-03ebcec6-1f9c-4218-b664-3245572bdcef.png">

## 3. Sentiment Analysis using NLTK Vader

![image](https://user-images.githubusercontent.com/91500767/172097203-200a4a0a-cad6-46c4-8268-d3ead94a1ade.png)

## 4. Regression Analysis

<img width="800" alt="image" src="https://user-images.githubusercontent.com/91500767/172097272-8d89fe08-e3cd-46dc-8533-8efcc69d229d.png">
<img width="800" alt="image" src="https://user-images.githubusercontent.com/91500767/172097277-a0d341d0-5c13-4c1f-9c81-69ecd5f5cf73.png">
<img width="800" alt="image" src="https://user-images.githubusercontent.com/91500767/172097331-f7b9ed6b-0776-4654-b333-76b4f9ae192c.png">
<img width="800" alt="image" src="https://user-images.githubusercontent.com/91500767/172097340-79efc1fb-2e83-492e-88b8-8e94cd1b3c77.png">

