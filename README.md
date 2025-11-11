#MovieLens Feature Engineering and Exploratory Data Analysis

#Overview
This project explores the MovieLens_dataset, focusing on feature engineering and exploratory data analysis to uncover meaningful patterns in user ratings and movie characteristics.  
The goal was to transform raw data into a structured dataset that could support the development of personalized recommendation systems.

Objectives
- Clean and merge datasets (movies, ratings, tags, and links)
- Handle missing values and duplicates effectively
- Create new features that describe user and movie behavior
- Explore relationships between ratings, genres, and movie age
- Identify insights that could guide future recommendation models


Dataset Description
The dataset used is a curated subset of the MovieLens database, containing:

| File | Description |
| movies.csv | Contains movie titles and genres |
| ratings.csv | Contains user ratings for each movie |
| tags.csv | Contains user-generated tags for movies |
| links.csv | Maps MovieLens IDs to IMDb and TMDb IDs |

A total of 100,818 ratings were analyzed across 9,711 movies from 610 users.


#Feature Engineering Highlights
New features were created to add analytical depth and support recommendation logic:

| Feature | Description | Purpose |
| release_year | Extracted from movie title (e.g., “Toy Story (1995)” → 1995) | Enables temporal analysis |
| movie_age | Years since release (2025 - release_year) | Distinguishes classics from modern films |
| num_genres | Number of genres per movie | Helps assess diversity in storytelling |
| main_genre | Primary genre of each movie | Simplifies content-based grouping |
| avg_movie_rating | Average rating per movie | Indicates general audience sentiment |
| num_ratings | Number of ratings per movie | Measures popularity and engagement |
| user_avg_rating | Average rating per user | Captures user rating tendencies |

These features combine to make the dataset ready for both collaborative filtering and content-based recommendation models.



#Exploratory Analysis & Insights
Key findings include:

1. Users rate positively overall: most ratings fall between 3.0 and 4.5, with an average of 3.5.  
2. Popular and Highly Rated: some lesser-known titles outperform mainstream hits in quality.  
3. Multi-genre films perform better, especially in recent years, reflecting modern audience tastes.  
4. Classic movies still shine: early films like The Immigrant (1917) and Aelita (1924) maintain high ratings.  
5. Dominant genres: Action, Comedy, and Drama lead in frequency, while Documentary and Adventure score higher on average.  
6. Evolving preferences: Viewers increasingly favor genre-blending and story-driven experiences.


#Tools Used
- Language: Python  
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, re  
- Environment: Google Colab / Jupyter Notebook  



#Deliverables
- Cleaned dataset with engineered features  
- Fully executed Jupyter Notebook (.ipynb)  
- Analytical report (.pd) summarizing methodology, features, and insights  


