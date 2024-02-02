# Portfolio | Python for Data Analysis
This portfolio aims to highlight Python skills and projects developed along my studies of Data Analysis.

## Table of Contents
1. Heat Map with Time using Folium
2. Interactive Dashboard with TKinter
3. Project: Clustering with K-Means
4. Project: Recommendation Systems

### 1. Heat Map with Time using Folium
 The Heat Map with Time is an interactive visualization that shows concentration of data over the time and, different from normal heat maps, this kind does not present relation between variables. It could also be used as an alternative for bar or line charts where it is wanted to express the gradual changes over the time.
 
 In this case I am using the NYC traffic accidents dataset in order to show in which time of the day there is higher occurrence of incidents. The dataset can be found at https://www.kaggle.com/datasets/mysarahmadbhat/nyc-traffic-accidents.
 
 Latitude and logitude data are needed to create the map and then a layer of time is added with a time indexed column. As result, we have an interactive map that presents the concentration of incidents happened by hour, where we can identify the time of the day with the highest and lowest car crashes. 
 
![image](https://user-images.githubusercontent.com/102151691/228522777-f0bcef81-33c6-4781-8aa1-c0338e6badbb.png)

 
 ### 2. Interactive Dashboard with TKinter
 TKinter might not be the most popular technology to create interactive dashboards but it is also an alternative for being easy to edit, where the main idea is to create a major function with sub categories to add functions inside the primary one, that will take form by using a mainloop().
 
 For this example I used data of book ratings and also data generated from APRIORI algorithm for Market Basket Analysis in order to demonstrate how to create a dashboard with TKinter. This dashboard was based on UX Design to older adults (65+) focusing on the contrast, as it is known that at this age their eyes get 40% less light, changing the vision. Additionally, titles and labels were set with large font size (12 or more) in order to better visualize the numbers.
 
![image](https://user-images.githubusercontent.com/102151691/228522824-f391c510-bb35-4487-a2c6-658291296d8e.png)

### 3. Project: Clustering with K-Means
 This project aimed to answer questions that would be important for a company that wants to publish new board games, in which its goal would be having a high average rating.
 
 Using PCA for feature importance, with a threshold of 0.25, was identified that the most important features for this analysis are: category, family and mechanic. As clustering works only for numerical data, word embedding process was needed to apply K-Means into the “category” in order to reduce the amount of unique values. To tokenize and remove stop words, I used “genism” library instead of NLTK, for being simpler to apply. From the same library, “Word2Vec” was used in order to learn and embed words, creating distance vectors, so then words that are similar in between would have a higher score. 
 
 As conclusion, was verified that if a company wants to publish a new board game, it’s more likely to have a higher score when the category is related to war, using mechanics of area control.

 ### 4. Recommendation Systems
 Application of Recommendation Systems (RS), using content-based and collaborative filtering, for suggestion of books:
 
 1. A search engine was created using content-based system, in which the summary of each book was used. The cosine similarity was calculated on a matrix created by the TfidfVectorizer algorithm, that transformed each summary into a vector. When typing a book that you like on the search engine, it returns ones that you might also like.
 2.The collaborative filtering item-item RS was created by using the NearestNeighbors algorithm, considering the rating of each book. Only books rated at least 50 times were considered in order to avoid bias.


