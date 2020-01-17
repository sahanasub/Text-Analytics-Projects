# Mine Your Own Business
## Lift Analysis of Car Brands
![cars](https://user-images.githubusercontent.com/44115595/72592498-4fb38080-38c8-11ea-9d5c-08884a4f23bd.PNG)

### Introduction
Today, the internet acts as a gathering place for users in the form of blogs, discussion forums and chat rooms, thereby generating massive amounts of data regarding the consumers' opinions, experiences and interactions. In this project, we explore the user-generated content from a car discussion forum - [Edmunds](https://forums.edmunds.com/) to analyze the consumers' preception of their car brand and the brand's competitors. We attempt to translate the user-generated content to market structure and competitive landscape insights.

### Technology
The project was implemented in Python 3.7.3.

#### Packages
* selenium
* nltk

### Approach
1. Scraped Edmunds forum for ~10k discussion posts about midsize sedans
2. Pre-processed the data and replaced individual card models with their respective brands and found the top 10 brands by frequency
3. Calculated the Lift ratios for associations between the brands and plotted the brands on a multi-dimensional scaling (MDS) map
4. Analyzed the association between the most frequently mentioned attributes and the top brands
5. Used Lift analysis to recognize the brands that consumers' consider aspirational

### Insights and Recommendations
* Ford's tagline "Go Further" is believed to have a dual meaning of being better than its competitors and improved fuel economy. Ford has a high lift with size but the lift with speed and power is relatively low. Given the company's emphasis on being better than their competitors, they need to improve the car in terms of power and speed.
* Ford is considered an affordable car by the company, but the public does not perceive this, evident by the low lift values(amongst other attributes and even amongst other competitors!) and hence they have to advertise the cars as affordable and low prices for its features. 
* Hyundai prides in high quality products but the lift value is very low, which is alarming. They need to look into quality issues and improve it to pass that important distinction it has from other competitiors to its customers. On the other hand, it is an affordable brand and it has high lift among its competitors with respect to price.
* People seem to asssociate Toyota with high quality which is a good news. It has the highest lift value amongst all its competitors. To help innovation resonate among its customers, they have to work on improving the cars in terms of power and speed.
* The Lift values indicate that Mercedes is the most aspirational brand, closely followed by Volvo. An important point to note is that for an aspirational brand like Mercedes, there is a fair probability that a large part of the audience who currently cannot afford it, might be able to afford it in the future. Being a luxury-brand, Mercedes can do well if they produce bottom-feeder lux models that can draw the mainstream audience to affordable luxury nameplates. Furthermore, Mercedes can also capitalize on leasing. Majority of the luxury cars are leased which is more affordable for the mainstream audience.



