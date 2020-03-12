# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Capstone Project: Recommender System for NBER Working Papers

### Problem Statement 


**To build a Working Paper Recommender System for users to provide relevant suggestions of working papers, almost similar to the queried working paper in terms of author, theme/program and title (topic of interest)**

---

### Executive Summary


Given that there is plethora of information available on the internet for any searched query, it is of utmost importance to provide users with only the relevant information. This information has to be similar to the characteristics of the searched query. This project aims to help researchers who are conducting literature review on any topic in the field of economics or development theory by suggesting them working papers similar to their queried paper. This would streamline the search and save time and effort put by users. The recommender system is easy to use and provides results quickly. 

For the purpose of building a Working Paper Recommender System, a dataset on authors and titles is forked from someone's github. On the other hand, the dataset on the program and working paper codes is scraped from the website of National Bureau of Economic Research (NBER). The dataset comprises of over 20,000 working papers written from 1975 to 2015, and spanning over 21 different themes/programs. The title and authors included in the corpus of working papers is cleaned for punctuations, english stopwords such as 'the','a','an',among others before sending to the built machine learning algorithm. The text of titles is also vectorized (that is converting each word into a number) to make it machine-readable. The recommender system uses cosine similarity to make recommendations about similar papers to the users when they input the title of any paper included in the dataset of NBER working papers. Cosine similarity is a metric used to measure similarity between any two texts/documents irrespective of their size/magnitude (length of the document). The closer the cosine similarity is to 1 between any working papers, more similar are the working papers. The project has built three recommender systems, namely, a) recommending papers only by title, b) recommending papers that have similar titles and authors, and c) recommending papers that have similar titles, authors and programs. After the user inputs a title, 10 most similar working papers are recommended from over 20,000 papers available in the corpus. 

Although the recommender system is easy to use and implement, it may have certain limitations. In this project, the recommender system is built solely on the content of titles and no information is used on user preferences for an author, theme, etc. To improve the robustness of the recommender system, it is essential to collect information about user preferences, and use more sphisticated techniques in deep learning to make the most suitable recommendations to the users in future. 

---

### Datasets 


The project uses the created datasets on the working papers published by the National Bureau of Economic Research over the period 1975-2015. The data for title and author is forked whereas for working paper code and program is scraped from the website using the BeautifulSoup Library. 

---

### Conclusion and Recommendations

The three recommender systems are making recommendations for working papers using title as an input. The users can search by titles and find other most similar working papers to the searched query. Whether the text is vectorized using count vectorizer or tf-idf vectorizer, the recommendations about the working papers are not significantly different (especially in the case of recommender system for a) title and author, and b) title, author and program). The recommender system is useful to academicians, students and others who are researching on any topic in the field of economics. Also, it could be employed as an e-library for searching working papers similar to the working paper of interest. The system is built to streamline search of relevant literature in plethora of information available on the website of NBER. 

One of the limitations of the model is that it is based only on the text of the titles of the working papers and no information about user preferences for programs, authors is included. The results of the model could be improved if more information about user profile is collected and modelled into the recommender system. Also, the recommender system can be extended to other fields such as science and social sciences. 
