# Twitter_Sentiment_Analysis_US_Presedential_Elction2020

**Objective: Using Python Script Extraction of tweets and Perform sentiment analysis on the presidential candidature of Donald Trump, Joe Biden before the elections in US in November, 2020.**
In this analysis extraction of tweets using Twitter's API, and GetOldTweets library to overcome the timeframe limitations of Twitter API is done. After extraction, I have done preprocessing for cleaning the datasets, basic EDA, sentiment analysis to observe polarity towards each candidate, used classification models on these sentiments and created visualizations.

**Data Preprocessing :** 
Data Preprocessing is a very crusial part for this project.Data preprocessing is the process of transforming raw data into a useful, understandable format.By preprocessing data, we make it easier to interpret and use. This process eliminates inconsistencies or duplicates in data, which can otherwise negatively affect a model’s accuracy. Data preprocessing also ensures that there aren’t any incorrect or missing values due to human error or bugs. In short, employing data preprocessing techniques makes the database more complete and accurate.
Steps to process the twitter data :

* Using Regular Expressions to remove Emojis from Tweets

* Using Regular Expressions to remove any retweets (if they exist)

* Using Regular Expressions to remove the usernames from the tweets as they do not provide any additional information

* Using Regular Expressions to remove any URLs, websites,etc

* Using Regular Expressions to identify for any hashtags in the tweet, & if they exist, remove the hashtag & keep the word. This can be very useful when modelling as it does not remove any possible words that might be a major factor in calculating the sentiment

* Using Regular Expressions to remove any special characters, numbers , punctuations

* Converting everything to lower case

* Lastly, used the Tweet-Preprocessor Module for cleaning any leftover junk.

Above portion is the main preprocessing part.Now for calculating sentiment perform certain task using NLTK module.Steps are given below:

* NLTK Module used to tokenize all words

* NLTK Module used for removing any existing stop words (eg. Or , from , them, Does , etc)

* NLTK Module used to perform stemming

* Words that less than a length of 2 were dropped

**Sentiment Analysis :**

Sentiment analysis is used to analyze raw text to drive objective quantitative results using natural language processing, machine learning, and other data analytics techniques. It is used to detect positive or negative sentiment in text, and often businesses use it to gauge branded reputation among their customers. 
Lexicon file is used to calculate the sentiment of each tweets.

**Donald Trump**

<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/Calculate%20Emotion%20of%20Users.png">
</p>
<h5>The above graph describe the Emotions of Users for Donal Trump</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/Count%20Of%20Tweets%20Per%20Day.png">
</p>
<h5>The above barplot is depicting the counts of tweets per day for Trump.The Y axis denotes the no. of tweets on the day of July 14 to July 21</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/Count%20Of%20Tweets%20Per%20Hour.png">
</p>
<h5>The above plot describe the No of tweets per hours on a particular day</h5>


<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/User%20Locations.png">
</p>
<h5>Shows the different locations of tweets</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/Source%20Of%20Tweets.png">
</p>
<h5>Source here refers to the medium used by the person to tweet, which can be Twitter Web App, Iphone, Android, ipad etc. Here we can see a major no. of user’s tweet using Web Application, followed by Iphone and the Ipad</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/Trump_SentimentOfTweetPerDay.png">
</p>
<h5>Given graph shows the No of tweets per day</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/Sentiments%20Of%20People%20Towards%20Trump.png">
</p>
<h5>This geographical map shows the sentiment of people around the country</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Donald%20Trump/WordCloud.png">
</p>
<h5> Word Cloud Representation</h5>



**Joe Biden**

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/Count%20Of%20Tweets%20Per%20Day.png">
</p>
<h5>The above barplot is depicting the counts of tweets per day for Trump.The Y axis denotes the no. of tweets on the day of July 14 to July 21</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/Count%20Of%20Tweets%20Per%20Hour.jpg">
</p>
<h5>The above plot describe the No of tweets per hours on a particular day</h5>


<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/User%20Locations%20For%20People%20Tweeting%20About%20Biden.png">
</p>
<h5>Shows the different locations of tweets</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/Source%20Of%20Tweets.png">
</p>
<h5>Source here refers to the medium used by the person to tweet, which can be Twitter Web App, Iphone, Android, ipad etc. Here we can see a major no. of user’s tweet using Web Application, followed by Iphone and the Ipad</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/Sentiment%20Of%20Tweets%20per%20Day.png">
</p>
<h5>Given graph shows the No of tweets per day</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/Sentiments%20Of%20People%20Towards%20Biden.png">
</p>
<h5>This geographical map shows the sentiment of people around the country</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/WordCloud.png">
</p>
<h5> Word Cloud Representation</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/Comparion%20Accuracy%20Score.png">
</p>
<h5>Comparison of Accuracy of Decision Tree,Random Forest and Naive Bayes for Joa Biden</h5>

<br>
<p align="center">
<img src = "https://github.com/Arupsau/Twitter_Sentiment_Analysis_US_Presedential_Elction2020/blob/main/Visualizations/Joe%20Biden/DL%20Train%20and%20Validation%20Accuracy.png">
</p>
<h5>Deep Learning based Training and Validation acuracy graph for Joe Biden </h5>
