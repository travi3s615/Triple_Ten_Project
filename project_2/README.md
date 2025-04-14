# Project Description

For this project, you’ll work with data from Instacart.

Instacart is a grocery delivery platform where customers can place a grocery order and have it delivered to them, similar to how Uber Eats and DoorDash work. This particular dataset was publicly released by Instacart in 2017 for a Kaggle competition. Although the original dataset is no longer available on the Instacart website, the version used here is a modified CSV version containing missing and duplicate values for learning purposes.

Your mission is to clean up the data and prepare a report that gives insight into the shopping habits of Instacart customers. After answering each question, a brief explanation of your results is required in a markdown cell of your Jupyter notebook.

You will generate plots that communicate your findings. Ensure that all plots have titles, labeled axes, and legends when appropriate. Use `plt.show()` at the end of each plot cell.

---

## Goal

Conduct Exploratory Data Analysis (EDA) on Instacart order data. You are expected to:
- Understand the structure and content of the dataset
- Preprocess missing or duplicate data
- Generate insights using statistics and visualizations
- Answer predefined analytical questions
- Summarize your conclusions

---

## Stages

The project consists of the following stages:

### 1. Data Overview
Examine the datasets:
- `instacart_orders.csv`
- `products.csv`
- `order_products.csv`
- `aisles.csv`
- `departments.csv`

Check for formatting issues, column names, missing values, and general structure.

### 2. Data Preprocessing
Perform:
- Data type corrections (e.g. convert IDs to `int`)
- Missing value identification and handling
- Duplicate record handling and explanation

Explain:
- What was missing/duplicated
- How you dealt with it
- Why the problem may have existed

### 3. Data Analysis
Perform and interpret visualizations and summary statistics to answer:
- When do customers place orders?
- How long do they wait between orders?
- Which products are most reordered?
- Which departments or aisles are most active?

Use sub-sections:
- [A] (must complete all)
- [B] (must complete all)
- [C] (must complete at least two)

---

## Finding

We found strong correlations among the most reordered and most purchased products. The top 8 commonly reordered products include bananas, strawberries, spinach, avocado, lemon and lime, raspberry, onion, and whole milk — indicating a preference for healthy food.

Out of all the top items in various queries (top 20 by order, reorder, and cart add), only 27 distinct products cover all major purchase behaviors. There’s a notable overlap between the top reordered and top purchased lists, with only slight differences, mostly in the order of purchase frequency.

---

## Note

This EDA project focused on order timing, frequency, and product popularity. The insights provided can help Instacart understand customer behavior and product trends.

All analysis was done using Python, with libraries such as:
- `pandas`
- `matplotlib`
- `seaborn`
- `numpy`

The project also emphasizes markdown-based documentation and clean, readable code.
