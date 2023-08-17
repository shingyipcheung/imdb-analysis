# imdb-analysis

## Overview

This notebook focuses on analyzing IMDb movie data, starting from the data acquisition phase (web scraping) to data visualization and conclusions. Here's a breakdown of the main sections and topics covered:

### 1. Web Scraping

In this section, the notebook provides code to scrape IMDb movie data. The following are the steps involved:
- Import necessary libraries like `requests`, `BeautifulSoup`, and `pandas`.
- Define a function (`scrape_page`) to scrape movie details from IMDb pages.
- Execute the scraping process for the first few IMDb pages and store the details in a list (`all_movies`).
- Convert the list of movie details into a pandas DataFrame for further analysis.

### 2. Preprocessing

The notebook emphasizes data cleaning and manipulation::
- Extracting the year from the 'Year' column and converting it to an integer.
- Ensuring the 'Metascore' column is of float type.
- Removing the "min" suffix from the 'Runtime' column and converting it to an integer.
- Using techniques like the `explode` function to handle list columns. This is particularly useful for columns like 'Genres' and 'Stars' that contain lists of values.

### 3. Visualization

This section delves deep into visualizing various aspects of the movie data:
- **Distribution of movie ratings and metascores over the years**: This visualization helps understand how movie ratings and metascores have trended over the years.
- **Most common genres and their correlation with ratings**: This visualization showcases the popularity of movie genres and how they relate to their respective ratings.
- **Average rating for each genre**: This helps in understanding which genres generally receive higher ratings.
- **Directors with the highest average movie ratings (with a minimum of 3 movies)**: This highlights the top-performing directors based on average movie ratings.
- **Relationship between movie runtime and its rating**: This visualization explores if there's any correlation between the length of a movie and its received rating.
- **Relationship between stars (actors) and movie ratings**: This aims to determine if certain actors consistently feature in highly-rated movies.

---
