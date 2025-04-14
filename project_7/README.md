# Project of Machine Learning

## Project Description

Mobile carrier Megaline has found that many of their subscribers are still using legacy plans. To improve customer satisfaction and increase profitability, the company aims to recommend one of two new plans—**Smart** or **Ultra**—based on customer behavior.

Your task is to build a **classification model** that analyzes users’ behavior and recommends the optimal plan. The data has already been preprocessed, so you can jump straight into modeling.

The goal is to achieve the highest possible **accuracy**, with a minimum threshold of **0.75**. Model performance will be validated using a test dataset.

---

## Data Description

The dataset `users_behavior.csv` contains monthly usage stats for each subscriber, including:

- `calls`: Number of calls made
- `minutes`: Total duration of calls (in minutes)
- `messages`: Number of text messages sent
- `mb_used`: Internet traffic used (in megabytes)
- `is_ultra`: Target variable (1 if Ultra plan, 0 if Smart plan)

---

## Project Instructions

1. Load and inspect the dataset.
2. Split the data into three sets: training, validation, and test.
3. Train multiple models, tweak hyperparameters, and compare their quality.
4. Evaluate the best-performing model using the test set.
5. Bonus: Sanity check the model—this data is trickier than usual!

---

## Evaluation Criteria

When this project is reviewed, attention will be given to the following:

- Quality of initial data exploration
- Proper dataset splitting into training, validation, and test sets
- Reasonable justification for chosen dataset sizes
- Accuracy and consistency of model evaluation
- Explanation of model choice and hyperparameter tuning
- Test results and final accuracy
- Adherence to project structure and clean, maintainable code

---

## Goal

Develop and validate a classification model that:
- Predicts whether a subscriber should use the Smart or Ultra plan
- Meets or exceeds an **accuracy score of 0.75** on the test set

---
