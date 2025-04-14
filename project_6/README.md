# Project on Analyzing Taxi and Weather Data

## Project Description

You're working as an analyst for Zuber, a new ride-sharing company launching in Chicago. Your task is to find patterns in taxi ride data to understand passenger preferences and how external factors such as weather affect ride frequency.

You'll work with a relational database and test a hypothesis regarding how weather impacts ride duration. The key focus is on analyzing competitor ride data and linking ride timestamps with weather conditions.

---

## Description of the Data

The database includes the following tables:

### `neighborhoods`
- `neighborhood_id`: Neighborhood code
- `name`: Name of the neighborhood

### `cabs`
- `cab_id`: Vehicle code
- `vehicle_id`: Vehicle's technical ID
- `company_name`: Taxi company

### `trips`
- `trip_id`: Ride code
- `cab_id`: Code of the cab used
- `start_ts`: Start timestamp of ride (rounded to the hour)
- `end_ts`: End timestamp of ride (rounded to the hour)
- `duration_seconds`: Duration of ride
- `distance_miles`: Ride distance
- `pickup_location_id`: Pickup neighborhood code
- `dropoff_location_id`: Dropoff neighborhood code

### `weather_records`
- `record_id`: Weather record code
- `ts`: Timestamp (rounded to the hour)
- `temperature`: Temperature during the record
- `description`: Weather condition description (e.g. "light rain", "scattered clouds")

**Note:** There is no direct link between `trips` and `weather_records`, but the data can be joined using timestamps from `trips.start_ts` and `weather_records.ts`.

---

## Instructions for Completing the Project

### Step 1: Parse Weather Data
Write a script to parse weather data for November 2017 from:
[Download Weather Dataset](https://practicum-content.s3.us-west-1.amazonaws.com/data-analyst-eng/moved_chicago_weather_2017.html)

---

## Step 2: SQL-Based Exploratory Data Analysis

1. **Rides by Company (Nov 15-16, 2017)**
   - Count rides per taxi company
   - Sort by `trips_amount` descending

2. **Companies with 'Yellow' or 'Blue' in Name (Nov 1–7, 2017)**
   - Filter companies by name
   - Count rides and group by `company_name`

3. **Popular Companies vs. Others**
   - Segment by company name
   - Group remaining companies as "Other"
   - Count rides per group and sort descending

---

## Step 3: SQL-Based Hypothesis Testing

### Hypothesis:
**"Duration of rides from the Loop to O’Hare changes on rainy Saturdays."**

Steps:
1. Get `neighborhood_id`s for Loop and O’Hare from `neighborhoods`
2. Retrieve weather conditions per hour from `weather_records`
   - Use `CASE` to define "Bad" weather if condition includes "rain" or "storm"
3. Get rides that:
   - Start in Loop (`neighborhood_id = 50`)
   - End in O’Hare (`neighborhood_id = 63`)
   - Occur on Saturdays
4. Join with weather and calculate `duration_seconds`

---

## Step 4: Python-Based EDA

Analyze results using:
- `project_sql_result_01.csv`: Contains `company_name` and `trips_amount`
- `project_sql_result_04.csv`: Contains `dropoff_location_name` and `average_trips`

Tasks:
- Import and inspect both datasets
- Verify data types
- Identify top 10 neighborhoods by drop-offs
- Visualize:
  - Rides per taxi company
  - Drop-offs per neighborhood

---

## Step 5: Hypothesis Testing (Python)

Analyze:
- File: `project_sql_result_07.csv`
- Columns: `start_ts`, `weather_conditions`, `duration_seconds`

### Hypothesis:
**"The average duration of rides from the Loop to O’Hare changes on rainy Saturdays."**

- Define null and alternative hypotheses
- Select test method (e.g. t-test or Mann-Whitney)
- Determine and apply `alpha` level
- Interpret result and draw conclusions

---

## Evaluation Criteria

Reviewers will assess:
- Data retrieval and slicing
- Grouping and joining accuracy
- Correct hypothesis formulation and testing
- Choice and justification of testing method
- Quality of conclusions
- Code structure and documentation

---
