# Project 1 | Project on IMDb Ratings

The project task was to analyze how the number of votes a show receives impacts its IMDb rating during the “Golden Age” of television. The goal was to test the assumption that highly-rated shows (we focused only on TV shows, ignoring movies) released during the “Golden Age” of television (starting in 1999 with *The Sopranos*) also have the most votes.

The project was split into three main phases:

# Stage 1: Data Overview
- Explored the dataset stored in `movies_and_shows.csv`
- Reviewed columns such as `title`, `type`, `genres`, `release_year`, `imdb_score`, and `imdb_votes`
- Identified which rows represented TV shows (not movies)

# Stage 2: Data Preprocessing
- Renamed and cleaned column names
- Removed duplicates and handled missing values
- Ensured all IMDb scores and votes were in the correct data type

# Stage 3: Data Analysis
- Focused only on TV shows released from 1999 onward
- Calculated trends and correlation between `imdb_score` and `imdb_votes`
- Determined whether the assumption held true based on average vote counts and rating distributions

# Goal
To validate the assumption:  
**"TV shows released during the 'Golden Age' of television receive the most IMDb votes and ratings."**

# Tools & Skills Used
- Python (Pandas, Matplotlib)
- Data cleaning and wrangling
- Hypothesis-driven exploratory data analysis
- Aggregation and visualization

---
