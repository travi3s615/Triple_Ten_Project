# Project of Analyzing Game Data

## Project Description

You work for the online store Ice, which sells video games globally. Your task is to analyze historical data on game sales, expert reviews, user reviews, genres, and platforms (e.g., Xbox or PlayStation) to identify patterns that determine game success. This analysis will help forecast trends and guide marketing efforts for the upcoming year — 2017 (with data up to 2016).

The dataset includes information about ESRB ratings, which assign age ratings such as "Teen" or "Mature."

---

## Goal

The key objective is to:

- Identify patterns in video game sales.
- Evaluate platform and genre performance.
- Determine the impact of critic/user reviews and ESRB ratings on sales.
- Recommend the most promising platforms and genres for 2017.

---

## Project Stages

### Step 1: Data Overview

- Load and examine the dataset `/datasets/games.csv`.
- Understand data types and column meanings.

### Step 2: Prepare the Data

- Convert all column names to lowercase.
- Change column types where necessary and justify the changes.
- Handle missing values:
  - Explain why they may be missing.
  - Describe how they are handled (filled or removed).
- Replace `TBD` user scores with `NaN` or another appropriate strategy.
- Calculate the total global sales (sum of all regions) for each game and add it as a new column.

### Step 3: Analyze the Data

- Games released per year: Is the data for each year sufficient?
- Platform performance:
  - Identify platforms with the most sales.
  - Observe how long it takes platforms to appear and fade.
- Focus on the relevant years for 2017 forecasting.
- Analyze platform trends:
  - Build distribution plots of global sales by platform.
  - Create boxplots to compare platforms.
- Correlation of reviews and sales:
  - Scatter plots of user vs. critic reviews for selected platform.
  - Calculate correlation coefficients.
- Compare the same games across different platforms.
- Genre trends:
  - Which genres sell the most?
  - Which genres have consistently low or high sales?

### Step 4: User Profile by Region

For each region (NA, EU, JP):

- Identify the top 5 platforms and their market differences.
- List the top 5 genres and compare across regions.
- Explore if ESRB ratings affect sales.

### Step 5: Hypothesis Testing

Test the following hypotheses:

1. Average user ratings of the Xbox One and PC platforms are the same.
2. Average user ratings for Action and Sports genres are different.

Explain:

- Null and alternative hypothesis formulation.
- Significance level (alpha) selection.
- Test methods and reasons for choice.

---

## Data Description

| Column Name     | Description |
|-----------------|-------------|
| `name`          | Game title |
| `platform`      | Console/platform name |
| `year_of_release` | Release year |
| `genre`         | Game genre |
| `na_sales`      | North America sales (USD million) |
| `eu_sales`      | Europe sales (USD million) |
| `jp_sales`      | Japan sales (USD million) |
| `other_sales`   | Other region sales (USD million) |
| `critic_score`  | Critic score (0–100) |
| `user_score`    | User score (0–10) |
| `rating`        | ESRB rating (e.g., "E", "M", "T") |

Note: Data for 2016 may be incomplete.

---

## Evaluation Criteria

Project reviewers will assess:

- Problem identification and data issues.
- Data preparation and handling.
- Clear and informative distribution visualizations.
- Correct statistical calculations (mean, variance, std).
- Hypothesis formulation and testing logic.
- Justified test methodology and result interpretation.
- Coherent and readable project structure.
- Insightful conclusions based on findings.
- Clean and commented code cells.

---
