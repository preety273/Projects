# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Reddit API, Classification and NLP


### Overview and Problem Statement 


A major cyber attack has temporarily rendered the Reddit website dysfunctional. This has also forced Reddit to explore  alternative mechanisms to perform its essential data classification functions. As a data scientist at reddit, I am tasked to build an alternative machine learning algorithm for accurately classifying the user posts into distinct subreddits or discussion topics depending on the content of the posts. For the purpose of a trial run in ascertaining the validity of the above algorithm, only posts from two subreddits are being trained and tested for the classification model.

---

### Executive Summary

This project focuses on data wrangling, natural language processing, and classification modelling for the random posts pulled from the two subreddits on the Reddit website. Reddit is a discussion website which allows users to post content and comments relating to a wide variety of fields ranging from day-to-day activities such as cooking to highly specialized domains such as Programming, Science, etc. I am a consultant with Reddit who has been tasked with developing an alternative machine learning algorithm which accurately classifies user-comments into specific categories depending on the content of each post. The user-content that is provided to me is related to Excel and Legal Advice subreddit. For the purpose of the project, I scrapped data (about 1,000 random user-posts for each subreddit) from the Reddit website. The data was later cleaned for punctuations as well as English stopwords such as is, are, and, among others for the purpose of building the model. Since the computer programs only accept an input in the form of digits, the entire textual dataset, comprising of title and posts, is converted into numbers using a function known as count vectorizer. The vectorizer provides a number corresponding to each word in the post and title according to its frequency, that is, the number of times a word appears in the title and the post. For simplication purposes, title and posts are combined together into a separate column called as "combined". Once the process of vectorization is complete, different models such as Logistic Regression, Naives Bayes and Decision Tree are fitted to the dataset. The models are further evaluated using the accuracy score. The comparison of all the three models indicates that Naives Bayes Model performs the best on the testing dataset. This model also showed a minor misclassification of the posts between the two subreddits. Only 1 post from Excel subreddit was misclassified as Legal Advice and vice-versa. Further research can be undertaken by employing more classification models such as Random Forest, Support Vector Machines, etc. and more observations can be added to see if the accuracy score improves.       

---

### Data


The project uses the scraped data from the Reddit website. The following subreddits scraped are - 
- Excel [https://www.reddit.com/r/excel/]
- Legal Advice [https://www.reddit.com/r/legaladvice/]

The datasets provide information about multiple variables such as title, selftext, subreddit, url, upvotes, among others from which only relevant variables are selected and a dataframe is made. 

---

### Data Dictionary


|Variable|Type|Description|
|---|----|----|
|title|object|title of the user-created posts|
|selftext|object|user-created posts|
|subreddit|object|user-created boards for posting related to excel and legal advice|

---

### Conclusion and Recommendations

The data for the subreddits - Excel and Legal Advice was scrapped from the Reddit website. Nearly 1,000 posts were scrapped, cleaned and analyzed for this classification project. A machine learning algorithm was developed to accurately classify the posts and titles from the two subreddits into distinct categories depending on their content. Three classification models namely, Logistic Regression, Naives Bayes, and Decision Tree, were fitted to the cleaned dataset (converted from words into numbers to provide as an input to the computer). A comprison of the results and speciafically the accuracy scores shows that Naives Bayes Model performs the best on the dataset. Only 1 post from the Excel subreddit was misclassified as a Legal Advice post and vice-versa. The accuracy score provided by the model was quite high given that the two subreddits are quite distinct. All of the three models used in the project are overfit and will not perform well on the unseen or new data. The project can be further expanded to include subreddits which are similar and also other classification models can be fitted and some measures such as tuning the hyperparameters can be taken to improve the predictive strength of the model so that it generalizes well. 

Given that the Naives Bayes Model provided the highest accuracy score for our dataset, it is recommended that the Reddit team employs this model because it fitted the dataset slightly better than the other models. However, the above mentioned steps need to be taken to stregthen the model. 
 
