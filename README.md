# Alcohol-Related Content on Social Media
Yu, C. (2022). MACS 30200 Final Project (Version 1.0.0) [Computer software]

**Pilot Findings:** \

**Sentiment analysis revealed that alcohol-related content on Twitter is slightly more positive than negative, while the positive and negative sentiment scores are similar but slightly more negative. According to the network analysis, the more similar the sentiment of two words are, the more likely they are in one post. On the other hand, there is an even distribution of subreddit communities based on their similarity and their sentiment scores.**


The code and data in this repository is an example of a reproducible research workflow for MACS 30200 "Perspectives on Computational Research" at the University of Chicago.

The code is written in Python 3.9.7 and all of its dependencies can be installed by running the following in the terminal (with the `requirements.txt` file included in this repository):
```
pip install -r requirements.txt
```

## **Alcohol-Related Content on Twitter**
Codes in `Scraping_Twitter.ipynb` can be used to scrape tweets that has the keyword `alcohol`.
You can then run codes in the jupyter notebook `Analysis_Twitter.ipynb` to replicate results in the final paper.

### Most frequent words associated with #alcohol
```
'alcohol', 'like', 'drink', 'people', 'drinking', 'drugs', 'get', 'one', 'time', 'know', 'good', 'would', 'think', 'even', 'drug', 'much', 'also', 'weed', 'drunk', 'never', 'use', 'need', 'make', 'day', 'go', 'free', 'life', 'want', 'really', 'take'
```
<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/169717226-fd8be2f5-e6fe-460d-bbf3-86fa1a468fce.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/169717256-247246cf-e3f1-479b-818c-16b555fdaf01.png">

### Sentiment Analysis
Positive, Negative, Neutral and Compound Sentiment Scores
```
The mean positive sentiment score: 0.168 (0.183)
The mean negative sentiment score: 0.138 (0.174)
The mena neutral sentiment score: 0.693 (0.22)
The mean compound sentiment score: 0.039 (0.486)
```

### Network Analysis
<img width="444" alt="image" src="https://user-images.githubusercontent.com/91500767/169717617-f0feea89-440d-4035-868a-68985e338466.png">
<img width="444" alt="image" src="https://user-images.githubusercontent.com/91500767/169717622-8fc65514-0b44-46c4-940e-3e398b5b8554.png">
<img width="444" alt="image" src="https://user-images.githubusercontent.com/91500767/169717627-957e8b3d-a572-4dcb-9e4e-eadb43997225.png">
<img width="444" alt="image" src="https://user-images.githubusercontent.com/91500767/169717630-7c8a0ae8-7c0d-4c42-8365-5f0836a9d9b4.png">


## **Alcohol-Related Content on Reddit**
Search results on `reddit.com` yields 56 subreddit communities most relevant to alcohol. Codes in `Scraping_Reddit.ipynb` can be used to scrape submissions and comments within those subreddit communities.
You can then run codes in the jupyter notebook `Analysis_Reddit.ipynb` to replicate results in the final paper.

### Most frequent words associated with alcohol
```
'like', 'get', 'people', 'one', 'would', 'time', 'good', 'know', 'think', "i'm", 'also', 'please', 'much', 'really', 'even', 'want', 'make', 'go', 'way', 'day', '...', 'r', 'need', 'going', 'see', 'drinking', 'feel', 'still', 'take', 'years'
```
<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/169717582-191651d9-d64a-4be1-9d6d-1f0d68ef87ea.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/91500767/169717586-bd4282d7-28f5-41f1-a0ff-d54f1fcf85cd.png">

### Sentiment Analysis
Positive, Negative, Neutral and Compound Sentiment Scores
```
The mean positive sentiment score: 0.036 (0.186)
The mean negative sentiment score: 0.036 (0.186)
The mena neutral sentiment score: 0.929 (0.258)
The mean compound sentiment score: -0.003 (0.108)
```

### Network Analysis
<img width="448" alt="image" src="https://user-images.githubusercontent.com/91500767/169717655-aaa9bf73-c520-4fbd-aecf-64aef7814202.png">
<img width="448" alt="image" src="https://user-images.githubusercontent.com/91500767/169717660-961f3b45-bed9-4459-9c33-cbe487faac23.png">
<img width="448" alt="image" src="https://user-images.githubusercontent.com/91500767/169717661-7b7bc98d-3f21-4583-9e3b-800dd663525b.png">
<img width="448" alt="image" src="https://user-images.githubusercontent.com/91500767/169717666-6250d7b3-2234-4127-8a9f-c3fc5bfb142c.png">
