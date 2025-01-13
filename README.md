# OTT Platform Movies Analysis

This project provides insights into the movies available on popular OTT platforms such as Netflix, Hulu, Prime Video, and Disney+. It focuses on analyzing the movie dataset and creating visualizations to better understand movie trends, including the application of K-Means clustering to group movies based on various features.

## Dataset

The dataset contains detailed information about movies available on OTT platforms. Key features include:

- **ID**: Unique identifier for each movie.
- **Title**: Movie name.
- **Year**: Year of release.
- **IMDb**: IMDb rating (between 1 and 10).
- **Rotten Tomatoes**: Rotten Tomatoes rating (percentage).
- **Netflix, Hulu, Prime Video, Disney+**: Boolean values indicating availability on each platform (True/False).
- **Type**: Type of movie (e.g., Movie, Documentary).
- **Genres**: List of genres (e.g., Drama, Action).
- **Country**: Country of production.
- **Runtime**: Duration of the movie in minutes.

## Sample Data

| Title        | Year | IMDb | Rotten Tomatoes | Netflix | Hulu | Prime Video | Disney+ | Runtime | Genres         |
|--------------|------|------|-----------------|---------|------|-------------|---------|---------|----------------|
| Movie A      | 2020 | 7.5  | 80%             | True    | False| True        | False   | 120     | Action, Comedy |
| Movie B      | 2019 | 6.3  | 65%             | False   | True | True        | True    | 100     | Drama, Thriller|
| Movie C      | 2021 | 8.0  | 90%             | True    | True | False       | True    | 130     | Comedy, Family |

## Tech Stack

- **Python**: Core programming language for analysis.
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **Scikit-Learn**: For machine learning, specifically K-Means clustering.
- **Plotly**: For interactive data visualizations.
- **Seaborn**: For advanced statistical visualizations.
- **Matplotlib**: For basic plotting and visualizations.

## Project Overview

This analysis aims to uncover patterns and trends in movie data across various OTT platforms. The project involved multiple visualizations, providing insights into the distribution of movies by genre, ratings, and runtime, as well as clustering analysis to identify similar movie groups based on key features.

### Key Steps in the Analysis:

1. **Data Preprocessing**: Cleaned and transformed the dataset, handling missing values, normalizing numeric features, and encoding categorical data.
2. **Data Visualizations**:
   - Visualized movie distribution across OTT platforms using bar and heatmap charts.
   - Explored relationships between IMDb ratings, Rotten Tomatoes scores, and runtime.
   - Created distribution plots to analyze the popularity and ratings of movies across platforms.
3. **K-Means Clustering**:
   - Applied the **K-Means clustering algorithm** on key features such as IMDb ratings, Rotten Tomatoes scores, and runtime to group movies into clusters.
   - The clustering model helped to identify patterns in movie characteristics (e.g., longer movies with higher ratings).
4. **Interactive Dashboards**: Utilized **Plotly** for creating interactive dashboards to visualize the movie distribution and clustering results.

## Clustering Analysis

- **K-Means Clustering** was used to group movies based on features like IMDb rating, Rotten Tomatoes score, and runtime.
- The clustering process involved selecting appropriate features, normalizing the data, and fitting the K-Means model to discover movie clusters.
- The model results showed distinct groups of movies with similar traits, helping to identify patterns based on movie ratings and runtime.

### Results of Clustering:

- **Cluster 1**: Movies with high IMDb ratings (>8), longer runtimes (>120 minutes), and high Rotten Tomatoes scores (80%+).
- **Cluster 2**: Movies with moderate IMDb ratings (6-7), medium runtimes (90-120 minutes), and moderate Rotten Tomatoes scores (70%-80%).
- **Cluster 3**: Movies with lower IMDb ratings (<6), shorter runtimes (<90 minutes), and lower Rotten Tomatoes scores (<70%).

The clustering process revealed that movies on OTT platforms can be classified into distinct groups based on key features, allowing for more targeted recommendations and insights for platform content strategies.

## Results

1. **Distribution of Ratings**: 
   - The dataset shows that the majority of movies have IMDb ratings between 6 and 8, with a few high-rated movies standing out in the upper range.
   
2. **Platform-Specific Trends**:
   - Netflix has a higher proportion of action movies, while Disney+ focuses more on family-oriented content.
   - Prime Video tends to feature a larger number of longer movies compared to other platforms.

3. **Clustering Insights**:
   - The clustering analysis helped identify groups of movies with similar characteristics, such as high ratings and long runtimes, providing a better understanding of content distribution and viewer preferences.

## Conclusion

This project offers valuable insights into the trends and patterns of movies available on OTT platforms. The use of K-Means clustering has helped uncover distinct groups of movies with similar characteristics, and the visualizations provide a clear view of how movies are distributed across platforms, their genres, and ratings. This analysis can assist in content strategy and recommendations for OTT providers.

