#Netflix Movies and TV Shows: Clustering

Project Summary :


- This project revolves around performing unsupervised clustering on a dataset of Netflix movies and TV shows. The dataset comprises information about each title, including the show ID, type (movie or TV show), title, director, cast, country of production, date added on Netflix, release year, rating, duration, genre, and description.

- The business context of this project stems from the observation that Netflix has experienced a significant increase in the number of TV shows available since 2010, while the number of movies has declined by over 2,000 titles during the same period. This trend sparks curiosity about what other insights can be derived from the dataset.

- To delve deeper into the analysis, external datasets like IMDB ratings and Rotten Tomatoes can be integrated to provide additional intriguing findings.

Challenges:

Exploratory Data Analysis: Analyzing a large dataset with multiple attributes and textual features to gain insights and identify patterns effectively.

Content Availability by Country: Understanding the types of content available in different countries and detecting variations and preferences.

Focus on TV Shows: Evaluating whether Netflix has shifted its focus towards TV shows and exploring trends in release years and the relative numbers of TV shows and movies.

Clustering Similar Content: Developing a clustering approach to group similar movies and TV shows based on titles, directors, cast, and descriptions.

Deliverables:

- Exploratory Data Analysis report providing insights and patterns from the dataset.
- Analysis of content availability across countries, highlighting variations and preferences.
- Evaluation of Netflix's focus on TV shows versus movies, supported by statistical analysis.
- Clustering results and interpretation, showcasing groups of similar content based on text-based features.


Success Criteria:

- Comprehensive exploratory data analysis, offering a clear understanding of Netflix's content landscape.
- Identification of variations in content availability across countries, aiding tailored offerings to different regions.
- Analysis confirming the focus shift towards TV shows and providing insights on the extent of the change.
- Effective clustering of similar content, demonstrating coherent groups with shared themes and genres.


Conclusion:


- In this project, we tackled a text clustering problem aimed at categorizing Netflix shows into distinct clusters based on their similarity. The dataset consisted of 7787 records with 11 attributes.

- To begin, we addressed missing values in the dataset and conducted exploratory data analysis (EDA). Our analysis revealed that Netflix primarily hosts movies and that the total number of shows added to the platform is growing exponentially. Additionally, a significant portion of the shows originated from the United States, and the majority of the content targeted adult and young adult audiences.

- We decided to cluster the data using attributes such as director, cast, country, genre, and description. These attributes were tokenized, preprocessed, and transformed into numerical features using TFIDF vectorization. This process resulted in a total of 20,000 attributes.

- To handle the curse of dimensionality, we employed Principal Component Analysis (PCA). Through analysis, we determined that 4,000 components were sufficient to capture over 80% of the variance, and therefore, we limited the number of components to 4,000.

- We employed the k-means clustering algorithm to build the initial clusters. Utilizing the elbow method and Silhouette score analysis, we determined that the optimal number of clusters was 6.

- Subsequently, we constructed clusters using the Agglomerative clustering algorithm, and the optimal number of clusters was determined to be 12 based on dendrogram visualization.To provide recommendations to users based on their watched shows, we developed a content-based recommender system using a similarity matrix obtained through cosine similarity.

- The recommender system generates 10 recommendations by considering the type of show the user has watched.

- Overall, this project involved data preprocessing, dimensionality reduction, clustering using k-means and Agglomerative algorithms, and the development of a content-based recommender system.
