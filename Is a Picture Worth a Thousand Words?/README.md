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

![summary](https://user-images.githubusercontent.com/44115595/72586525-b8dec800-38b7-11ea-9e53-acd501c38420.PNG)

### Insights and Recommendations

Based on the regression analysis, the best model (AU-ROC: ~0.72) to predict user engagement was using both the image captions and the image labels. 
* The Instagram caption does bear some weight in determining engagement, but is not necessarily sufficient, as captions may be slightly unrelated to the actual image. Combining these captions with the labels from Google Cloud Vision, we are able to better predict engagement, as Google Vision has already been exposed to a variety of images that can then be used to determine the labels.

Based on LDA, we can see that many of the posts fall under the main category of Nature. There are many overlaps within these topics, given that most are related to nature, landscapes and animals. People expect these photos from NatGeo, and these photos are probably the reason they are actively following the account. NatGeo is first and foremost known for their nature based magazines, which have been a household name since 1888. The Instagram account is an extension of this brand image they have created in homes, and thus, it is essential to maintain that on different platforms as well. However, there is also room to engage with a new userbase through Instagram, which is why we recommend slowly starting to add in a mix of new images corresponding to other topics.
* The high engagement posts mostly relate to wildlife and atmospheric phenomena. NatGeo can try increasing the frequency of these topics to drive engagement
* The low engagement posts consists mainly of the most commonly occuring theme - nature. Though these are frequent, these posts don't seem to garner much enthusiasm

One thing that could be useful to monitor is how the trends in engagement topics change based on season. For example, more individuals might engage with travel related images prior to planning a trip, which would cause an increase in certain topic label engagement. They may also want to see more images of people/human elements of emotion during the holidays, and pictures of sunny warm places in the winter. Looking at how engagement changes by season in general could be a great way to drive engagement by posting more targeted images at certain times of the year.
