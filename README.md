# Netflix Movie Data Analysis

## Problem Statement

Netflix uses data-driven insights to improve its content strategy and recommendation algorithms. This project analyzes a dataset of over 9,800+ movies to address key business questions related to genre trends, popularity, audience engagement, and production timelines.The goal is to provide actionable insights for content acquisition and personalized recommendations.

## Objectives

This project aims to analyze Netflix movie data to answer the following:

1.  **Content Trends:** Identify the most frequent genres and yearly production patterns.
   
2.  **Audience Preferences:** Determine genres/movies with the highest votes and popularity.
   
3.  **Strategic Insights:** Highlight underperforming genres and peak production years.

## Dataset Overview

* Initial Size: 9,827 rows × 9 columns.
* Cleaned Data: 9,827 rows × 6 columns after preprocessing.
* Key Columns: `title`, `genre`, `release_year`, `popularity`, `vote_average`, `Vote_count`

## Tools & Technologies

* **Language:** Python
* **Libraries:**
    * `Pandas` (data manipulation)
    * `Matplotlib`/`Seaborn` (visualization)

## Steps Involved

The analysis involved the following steps:

1.  **Data Loading and Exploration:**
    * Loaded the dataset using Pandas (`pd.read_csv`).
    * Explored the dataset's structure using `df.head()`, `df.info()`, `df.describe()`, and `df.shape`.
    * Identified data types and missing values.
    * Checked for duplicated values.

2.  **Data Cleaning and Preprocessing:**
    * Converted the `Release_Date` column to datetime format and extracted the year.
    * Dropped unnecessary columns (`Overview`, `Original_Language`, `Poster_Url`).
    * Categorized the `Vote_Average` column into bins: 'not\_popular', 'below\_avg', 'average', and 'popular'
    * Handled genre data by splitting genre strings into lists and exploding the dataframe so each movie has one genre per row.

3.  **Exploratory Data Analysis (EDA):**
    * Determined the most frequent movie genres.
    * Identified movies with the highest and lowest popularity.
    * Analyzed the distribution of vote averages.
    * Determined the year with the most movie releases.

4.  **Data Visualization:**
    * Visualized genre frequencies.
    * Visualized popularity.
    * Visualized vote averages.
    * Visualized movie releases by year.

## Key Findings

* Drama is the most frequent genre in the dataset, appearing more than 14% of the time.
* 25.5% of the dataset has movies with "popular" vote averages.
* Drama is the most popular genre among fans, with over 18.5% of movies.
* "Spider-Man: No Way Home" has the highest popularity and belongs to the Action, Adventure, and Science Fiction genres.
* The year 2020 has the highest number of movie releases.

## Libraries Used

* Pandas
* Numpy
* Matplotlib
* Seaborn

## Conclusion

This analysis provides insights into Netflix movie data, including genre trends, movie popularity, and release patterns. The findings can be used to inform content acquisition strategies and improve recommendation systems.
