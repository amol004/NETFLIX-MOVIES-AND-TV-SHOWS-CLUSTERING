# Problem Statement
The objective of this project is to group Netflix's content according to site data. Clustering the video content would not only help construct an effective recommendation system but also reveal what kind of content the company is interested in displaying on its website. Providing filmmakers and content developers with an understanding of the kind of video content that consumers want.


![344395594-8c2d7664-4f4a-4821-a8af-77906a824c01](https://github.com/user-attachments/assets/1753a7cd-2d97-4074-82fd-1d35b0006500)

# Objective
The main objective of this project is to analyze the Netflix dataset to identify trends and patterns in the content available on the platform. The insights derived will be utilized to improve user experience and guide recommendations for future content.

# Dataset
The dataset includes a collection of movies and TV shows available on Netflix as of 2019, containing approximately 7,787 records and 11 attributes.

# Data Pipeline
## Data Understanding: 
Initially, the dataset was examined to understand its features, structure, and to identify any potential patterns or trends. This involved analyzing the data shape, the data types of each feature, and summarizing the statistics.

## Exploratory Data Analysis (EDA):

An exploratory analysis was conducted to identify patterns and dependencies within the data, providing a basis for further processing. Data Cleaning: The dataset was cleaned by checking for duplicate values, handling null values and outliers, and imputing missing data where necessary.

## Text Data Preprocessing : 
Textual data was prepared for clustering by using techniques such as stop word removal, punctuation removal, conversion to lowercase, stemming, tokenization, and word vectorization. Principal Component Analysis (PCA) was applied to manage the dimensionality.

## Clustering Implementation: 
K-Means and Agglomerative Hierarchical clustering algorithms were used to group the movies, with the optimal number of clusters being determined through various methods.

## Content-Based Recommendation System:
A content-based recommendation system was developed using the similarity matrix obtained from cosine similarity, which provides users with 10 recommendations based on the type of content they have watched.

# Conclusion
The project successfully identified several trends and patterns in the Netflix dataset, offering insights that can be leveraged to enhance user experience and inform future content recommendations:

Netflix has a larger library of movies compared to TV shows, and the number of new additions to Netflix is growing rapidly.

The majority of the content is produced in the United States.

Attributes such as cast, country, genre, director, rating, and description were used for clustering.

The TFIDF vectorizer was employed to tokenize, preprocess, and vectorize these attributes, resulting in the creation of 10,000 features.

PCA was utilized to address dimensionality, reducing the total number of components to 3,000, which accounted for over 80% of the variance.

The optimal number of clusters was found to be 6 using K-Means Clustering, determined by the elbow method and Silhouette score analysis.

Using Agglomerative clustering, the optimal number of clusters was identified as 7, as visualized through the dendrogram.

A content-based recommender system was built using the similarity matrix generated by cosine similarity, offering users ten recommendations based on the type of content they watched.
