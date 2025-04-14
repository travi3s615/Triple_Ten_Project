# Statistical Data Analysis

## Project Description

You work as an analyst for the telecom operator **Megaline**, which offers two prepaid plans: **Surf** and **Ultimate**. The commercial department wants to identify which plan brings in more revenue so they can adjust their marketing strategy accordingly.

Your job is to conduct a **preliminary analysis** of client behavior using a dataset of 500 Megaline clients from 2018. The data includes which plan users subscribed to, how many calls/texts they made, and how much internet they used.

The project’s goal is to determine which plan is more profitable and provide recommendations based on statistical testing and exploratory data analysis.

---

## Description of the Plans

### Surf Plan:
- Monthly charge: **$20**
- Includes: 500 mins, 50 texts, 15 GB data
- After limits:
  - 1 minute = $0.03
  - 1 text = $0.03
  - 1 GB = $10

### Ultimate Plan:
- Monthly charge: **$70**
- Includes: 3000 mins, 1000 texts, 30 GB data
- After limits:
  - 1 minute = $0.01
  - 1 text = $0.01
  - 1 GB = $7

---

## Project Process

### Step 1: Prepare the Data
- Convert columns to appropriate data types.
- Identify and remove errors or inconsistencies.
- Calculate:
  - Number of calls, texts, and web sessions per user per month.
  - Monthly revenue per user (accounting for limits and plan pricing).

### Step 2: Analyze the Data
- Plot histograms and distributions.
- Compute descriptive statistics (mean, variance, standard deviation).
- Compare customer behavior between plans.

### Step 3: Hypothesis Testing
Test the following:
1. The **average revenue** from Surf vs Ultimate plan users differs.
2. The **average revenue** from NY-NJ users differs from other regions.

Use an appropriate significance level (α) and statistical test (likely two-sample t-test).

---

## General Conclusion

- The **Ultimate** plan yields **higher average revenue per user**, despite users underutilizing the full quota of calls/texts/data.
- **Surf** users frequently exceed their plan limits, resulting in **additional charges** that increase revenue.
- Most revenue comes from users exceeding limits or having skewed usage patterns (Pareto principle observed).
- Distributions:
  - Surf plan shows **right-skewed normal** for messages and data.
  - Ultimate plan shows **more uniform** distribution.

---

## Suggestions for Megaline

1. Encourage **Ultimate plan users** to increase usage of free services (loyalty incentive).
2. Adjust **Surf plan limits or pricing**, or introduce a **mid-tier plan** to better capture revenue potential from heavy users.

---

## Next Steps

- Explore **churn data** to assess long-term plan retention.
- Evaluate behavior by **age group**, **city**, or other demographic factors.
- Improve models with **additional months of data** if available.

