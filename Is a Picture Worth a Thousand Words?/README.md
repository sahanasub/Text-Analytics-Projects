# Is a Picture Worth a Thousand Words?
## Instagram User Engagement Analysis
![instagram-analytics-insights](https://user-images.githubusercontent.com/44115595/72576346-11509e00-3895-11ea-8883-8e4c5b77ba72.png)

### Introduction
The world is riding the social media wave and with more than 2 billion active social media profiles, businesses are increasingly switching to social media to reach out to their audience and build their brand presense. If we consider the most popular one, Instagram is outshining all other platforms. This comes as no surprise because visual storytelling is the best way to communicate and get your message across to the people.

In this project, we analyze the posts of a popular Instagram account - [National Geographic](https://www.instagram.com/natgeo/?hl=en) and attempt to predict user engagement (weighted metric of likes and comments) using the post captions and the image labels derived from Google Vision API. 

### Technology
The project was implemented in Python 3.7.3.

#### Packages
* gensim
* nltk
* spacy
* google.cloud.vision
* BeautifulSoup

### Approach
1. Extracted Instagram posts (image links, number of likes, number of comments and image captions) using BeautifulSoup
2. Used the Google Vision API to detect the labels for the images
3. Built Logistic Regression models to predict the engagement and derive insights
4. Topic Modeling using Latent Dirichlet Allocation (LDA) on the image labels to discern popular topics

### General Summary


### Insights and Recommendations
