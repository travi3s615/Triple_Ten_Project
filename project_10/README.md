# Gold Recover Prediction

# Project 10: Predicting Gold Recovery Efficiency

## Project Description

In this project, you're working with a dataset from a gold mining operation. The goal is to create a model that can predict the efficiency of gold recovery at various stages of the production process. You are provided with:

- `gold_recovery_train.csv` — training dataset  
- `gold_recovery_test.csv` — test dataset  
- `gold_recovery_full.csv` — full source dataset  

>  Some parameters are only present in the training set and calculated later in the process. Therefore, they are missing from the test set.

Each observation includes a `date` timestamp, and parameters measured close together in time tend to be similar.

The test set does not include target features, so the model's performance will be validated using the source dataset.

Before training the model, you must verify data quality and calculate the **final sMAPE** value based on two targets:
- `rougher.output.recovery`
- `final.output.recovery`

The final score is calculated using the following formula:

![image](https://github.com/user-attachments/assets/ed96d07f-3912-4653-8a22-2f5ff89af5bd)

## Project Instructions

### 1. Prepare the Data

1. Open and review the following files:
    - `/datasets/gold_recovery_train.csv`
    - `/datasets/gold_recovery_test.csv`
    - `/datasets/gold_recovery_full.csv`

2. Check the recovery calculation:
    - Use the training set to calculate `rougher.output.recovery`.
    - Compare your calculation to the existing value using **MAE**.
    - Provide findings.

3. Analyze the features missing from the test set.
    - What are they?
    - What types are they?

4. Preprocess the data:
    - Handle missing values
    - Standardize columns
    - Clean anomalies

---

### 2. Analyze the Data

1. Analyze how metal concentrations (Au, Ag, Pb) change at different purification stages.

2. Compare feed particle size distributions in the training and test datasets.
    - If distributions differ significantly, model quality may suffer.

3. Analyze total concentrations of all substances at different stages:
    - raw feed
    - rougher concentrate
    - final concentrate

    If you find abnormal values, investigate and remove them.

---

### 3. Build the Model

1. Implement a function to calculate the **sMAPE** metric:

![image](https://github.com/user-attachments/assets/c9e64fd8-d249-43e8-8387-2030fa956b0a)

2. Train models:
    - Use **cross-validation**
    - Compare performance
    - Select and test the best model on the test set

3. Compute and report the **final sMAPE** using:
    - 25% for `rougher.output.recovery`
    - 75% for `final.output.recovery`

---

## Project Evaluation

Reviewers will assess the following:

-  Have you properly prepared and analyzed the data?
-  What models did you try?
-  How did you evaluate model quality?
-  Did you follow all the instructions and structure?
-  What are your conclusions and insights?
-  Is the code clean and free of duplication?

---

## Summary

This project demonstrates your ability to:

- Handle real-world, imperfect data
- Evaluate data quality and distributions
- Train regression models using cross-validation
- Apply custom evaluation metrics
- Communicate findings clearly


