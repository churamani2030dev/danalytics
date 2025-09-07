# danalytics
# Movie Data Analysis

This notebook analyzes movie data from the [TMDB 5000 Movie Dataset](https://www.kaggle.com/tmdb/tmdb-movie-metadata). The goal is to extract and analyze information about cast, crew, genres, and keywords, and visualize the findings.

## Analysis Steps

1.  **Data Loading**: Loaded the `tmdb_5000_credits.csv` dataset. An attempt was made to load `tmdb_5000_movies.csv` but the file was not found in the expected directory.
2.  **Data Exploration**: Displayed the head, info, and checked for null values in the `df_credits` DataFrame.
3.  **JSON Parsing**: Parsed the 'cast' and 'crew' columns (which are in JSON format) to extract actor names, character names, and director names.
4.  **Exploratory Data Analysis (EDA)**: Calculated the frequency of cast and directors to identify the top entities in these categories.
5.  **Visualization**: Created bar plots to visualize the top 10 most frequent cast members and directors.
6.  **Summarization**: Summarized the key findings and limitations of the analysis.

## Key Findings

Based on the analysis of the `tmdb_5000_credits.csv` dataset:

*   The dataset contains information on movie IDs, titles, cast, and crew for 4803 movies.
*   The 'cast' and 'crew' columns were successfully parsed.
*   The top 10 most frequent cast members and directors were identified and visualized.

**Top 10 Most Frequent Cast Members:**

*   Samuel L. Jackson: Appeared in 67 movies
*   Robert De Niro: Appeared in 57 movies
*   Bruce Willis: Appeared in 51 movies
*   Matt Damon: Appeared in 48 movies
*   Morgan Freeman: Appeared in 46 movies
*   Steve Buscemi: Appeared in 43 movies
*   Liam Neeson: Appeared in 41 movies
*   Johnny Depp: Appeared in 40 movies
*   Owen Wilson: Appeared in 40 movies
*   John Goodman: Appeared in 39 movies

**Top 10 Most Frequent Directors:**

*   Unknown: Directed 30 movies
*   Steven Spielberg: Directed 27 movies
*   Woody Allen: Directed 22 movies
*   Martin Scorsese: Directed 21 movies
*   Clint Eastwood: Directed 20 movies
*   Robert Rodriguez: Directed 17 movies
*   Ridley Scott: Directed 16 movies
*   Spike Lee: Directed 16 movies
*   Steven Soderbergh: Directed 15 movies
*   Renny Harlin: Directed 15 movies

## Limitations

*   A comprehensive analysis including top genres and keywords could not be performed because the `tmdb_5000_movies.csv` file was not found.

## Next Steps

*   Obtain the `tmdb_5000_movies.csv` file and place it in the `/content/` directory to perform a complete analysis including genres and keywords.
*   Further investigate the "Unknown" director category to understand the extent of missing data.
*   Explore potential collaborations between top cast members and directors.
