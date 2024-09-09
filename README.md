# Problem Statement
The objective of this project is to group Netflix's content according to site data. Clustering the video content would not only help construct an effective recommendation system but also reveal what kind of content the company is interested in displaying on its website. Providing filmmakers and content developers with an understanding of the kind of video content that consumers want.


![344395594-8c2d7664-4f4a-4821-a8af-77906a824c01](https://github.com/user-attachments/assets/1753a7cd-2d97-4074-82fd-1d35b0006500)

# Objective
The main objective of this project is to analyze the Netflix dataset to identify trends and patterns in the content available on the platform. The insights derived will be utilized to improve user experience and guide recommendations for future content.

# Dataset 
The dataset includes a collection of movies and TV shows available on Netflix as of 2019, containing approximately 7,787 records and 12 attributes.
## Variables Description
### 1. show_id : Unique ID for every Movie / Tv Show

### 2. type : Identifier - A Movie or TV Show

### 3. title : Title of the Movie / Tv Show

### 4. director : Director of the Movie

### 5. cast : Actors involved in the movie / show

### 6. country : Country where the movie / show was produced

### 7. date_added : Date it was added on Netflix

### 8. release_year : Actual Releaseyear of the movie / show

### 9. rating : TV Rating of the movie / show

### 10. duration : Total Duration - in minutes or number of seasons

### 11. listed_in : Genere

### 12. description: The Summary description

# Data Pipeline
### Data Understanding: 
Initially, the dataset was examined to understand its features, structure, and to identify any potential patterns or trends. This involved analyzing the data shape, the data types of each feature, and summarizing the statistics.

### Exploratory Data Analysis (EDA):

An exploratory analysis was conducted to identify patterns and dependencies within the data, providing a basis for further processing.The dataset was cleaned by checking for duplicate values, handling null values and outliers, and imputing missing data where necessary.

### Text Data Preprocessing : 
Textual data was prepared for clustering by using techniques such as stop word removal, punctuation removal, conversion to lowercase, stemming, tokenization, and word vectorization. Principal Component Analysis (PCA) was applied to manage the dimensionality.

### Clustering Implementation: 
K-Means and Agglomerative Hierarchical clustering algorithms were used to group the movies, with the optimal number of clusters being determined through various methods.

### Content-Based Recommendation System:
A content-based recommendation system was developed using the similarity matrix obtained from cosine similarity, which provides users with 10 recommendations based on the type of content they have watched.

# Conclusion
In this project, we explored various machine learning techniques to analyze a dataset containing information about movies and TV shows. We performed data cleaning, preprocessing, feature engineering, and dimensionality reduction to prepare the data for modeling.

### Insights from EDA:

1.International movies is the top genre followed by Dramas and Comedies.

2.Movies and TV Shows on Netflix are in ratio 7/3. And TV Shows have long way to catch upto the number of Movies as movies are more popular than TV shows.

3.Most content on Netflix is from United States followed by India and United Kingdom.

4.Raul Campos and Jan Suter together directed 18 movies. We can observe some other great names such as Jay Chapman, Martin Scorsese and Steven Spielberg in top 20 directors list.

5.Most movies are of length ~100 mins while most TV Shows have only one season.

6.Most content on Netflix is rated for mature audience only.

7.From October to January, maximum number of movies and TV shows were added on the platform.

8.The most popular language is English, followed by Hindi and Spanish.

9.The majority of movies and TV shows have a duration between 80 and 120 minutes.

10.There are a small number of movies and TV shows with very short or very long durations.

### Insights from PCA:

1.The first 4750 principal components explain 90% of the variance in the data.

2.This suggests that the data is relatively high-dimensional, but that most of the information can be captured by a relatively small number of features.

3.This can be useful for reducing the dimensionality of the data for downstream tasks, such as clustering or classification.

### Insights from K-means clustering:

1.The optimal number of clusters according to the elbow method is 3.

2.The optimal number of clusters according to the silhouette method is 5. This suggests that the data can be reasonably well-clustered into 3 or 5 groups ,clusters are relatively well-separated, as 
indicated by the silhouette scores.

3.The most popular cluster is cluster 0, which contains a mix of movies and TV shows.

4.The other clusters are more specialized, containing mostly movies or TV shows.

### Insights from hierarchical clustering:

1.The optimal number of clusters according to the dendrogram is 6.

2.This suggests that the data can be reasonably well-clustered into 6 groups.

3.The clusters are relatively well-separated, as indicated by the distances between the clusters in the dendrogram.

4.The most popular cluster is cluster 0, which contains a mix of movies and TV shows.


### Insights from the recommender system:

1.The recommender system is able to generate relevant recommendations based on the cosine similarity between movies and TV shows.

2.The recommendations are based on the content of the movies and TV shows, rather than on their popularity or other factors.

3.This can be useful for users who are looking for new and interesting content to watch.
