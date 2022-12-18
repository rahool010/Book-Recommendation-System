
<h1 align="center">  Book Recommendation System
 </h1>

<h3 align="center"> AlmaBetter Verified Project - <a href="https://www.almabetter.com/"> AlmaBetter School </a> </h5>


![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Project Summary
With traditional methods of reading being replaced by the world on the web, recommendation systems have become a necessity more than just a luxury. The use of recommender system has a significant impact on the sales of various products and services. More and more companies are investing in building recommendation systems to engage users by providing them with personalized recommendations which depend on the users’ own behaviors. These systems have proved to be a significant part in boosting sales of various companies.

The main objective of this project is to create a Book recommendation system that best predicts user interests and recommend the appropriate books to them using various approaches.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Problem Statement
Recommender systems are widely employed in industry and are ubiquitous in our daily lives. Many worldwide known industry leaders save billions of dollars and engage several times more users be harnessing the power of recommender systems. Hence, Netflix says they save $1 billion each year, and around 75% of content users get through recommendations. These systems are utilized in a number of areas, Online book selling websites nowadays are competing with each other by many means.One of the most effective strategies for increasing sales,enhancing customer experience and retaining customers is building an efficient Recommendation system. The book recommendation system must recommend relevant books to read,so as to create a delightful user experience. Popularity based approach and Collaborative filtering approach are used in this project to build book recommendation systems.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Dataset Information
**Users**

User-ID: A unique identification number for each user
Location:It contains city,state and country to which the user belongs ,separated by commas
Age:The age of the user

**Books**

ISBN:International Standard Book Number unique to each edition of the book
Book-Title:Title of the book
Book-Author:Author of the book(incase of several authors only the first is provided)
Year-of-Publication:The year in which the particular edition of the book was published
Publisher:Name of the Book Publishing company
Image-URL-S: URL link to a small version of the book cover displayed on the Amazon website
Image-URL-M: URL link to Medium version image of the book cover displayed on the Amazon website
Image-URL-L: URL link to Large sized image of the book cover displayed on the Amazon website

**Ratings**

User-ID:as mentioned above
ISBN:as mentioned above
Book-Rating: The rating given by the user (identified by User-ID) for the book (identified by ISBN). It is either explicit,expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit,expressed by 0.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Tools and Technologies used
The programming language used in this project is Python. The following libraries were used for data analysis and data visualization and to build a recommender system.

* **Pandas** : For loading the dataset and performing data wrangling.
* **Matplotlib**: For data visualization.
* **Seaborn**: For data visualization.
* **NumPy**: For some math operations in predictions.
* **Statsmodels**: For statistical computations.
* **Sklearn**: For the purpose of analysis, prediction and evaluation.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Steps
* **Data Preprocessing** : Checked for outliers, incorrect values, missing values, duplicate, performed data type correction and string formatting.
* **Merging of datasets** : In this project, recommender systems were built utilizing only explicit ratings . So finally,a new dataframe by merging the books dataset ,explicit ratings dataset and users dataset.
* **Feature Extraction** : Created new columns such as age_group by binning the 'Age' column and extracted the country name from the 'Location' column .
* **Exploratory Data Analysis** : Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.
* **Implementation of various Recommender System approaches.**

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Approaches Used
The approaches used in this project are:
    
1. Popularity Based recommendation system

It is a type of recommendation system which works on the principle of popularity and or anything which is in trend. These systems check about the book which are in trend or are most popular among the users and directly recommend them.

2. Collaborative Filitering Based recommendation system

The collaborative filtering approach is the most popular technique used in Recommendation Systems. This filtering method is usually based on collecting and analyzing information on user’s behaviors, their activities or preferences, and predicting what they will like based on the similarity with other users. This approach is based on the following hypothesis: people who agreed with a user in the past will also agree in the future.

CF is broadly classified as memory-based and model-based CF.

#### Memory Based approach - KNN (similarity between items)
    
Memory-based methods use user rating historical data to compute the similarity between users or items. The idea behind these methods is to define a similarity measure between users or items, and find the most similar to recommend unseen items.

#### Model Based approach- SVD based recommendation system (prediction of ratings)

The matrix factorization technique ‘factorizes’ the user-item matrix into rectangular matrices of lower dimension. In particular, this approach uses Singular Value Decomposition. In this approach what we broadly do is set forth a pivot table with Customers and Items as columns and rows, and values for each customer-Item mapping is either a zero or an explicit rating for that particular customer-item pair. This matrix is then decomposed into factors using SVD and the individual element of decomposition is multiplied back into a complete matrix to finally generate recommendations.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Conclusion
* "Selected Poems" were read more by the users.
* Majority of the users are from USA and Canada.
* "Harlequin" has published the most number of books.
* Among Authors, "Agatha Christie" has written the most number of books followed by "William Shakespeare" and "Stephen King".
* After evaluation for Collaborative-Model Based Recommendation system, we got a recall@5 of 31% and recall@10 of 43%.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)