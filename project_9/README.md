# Project of Finding the Best Well

# Project Description

You work for the OilyGiant mining company. Your task is to find the best place for a new well.

## Steps to choose the location:
- Collect the oil well parameters in the selected region: oil quality and volume of reserves;
- Build a model for predicting the volume of reserves in the new wells;
- Pick the oil wells with the highest estimated values;
- Pick the region with the highest total profit for the selected oil wells.

You have data on oil samples from three regions. Parameters of each oil well in the region are already known. Build a model that will help to pick the region with the highest profit margin. Analyze potential profit and risks using the **Bootstrapping** technique.

---

# Project Instructions

### Step 1: Prepare the data
1. Download and prepare the data. Explain the procedure.

### Step 2: Train and test the model for each region
2.1. Split the data into a training set and validation set at a ratio of 75:25  
2.2. Train the model and make predictions for the validation set  
2.3. Save the predictions and correct answers for the validation set  
2.4. Print the average volume of predicted reserves and model RMSE  
2.5. Analyze the results  

### Step 3: Prepare for profit calculation
3.1. Store all key values for calculations in separate variables  
3.2. Calculate the volume of reserves sufficient for developing a new well without losses. Compare the obtained value with the average volume of reserves in each region  
3.3. Provide the findings about the preparation for profit calculation step  

### Step 4: Write a function to calculate profit
4.1. Pick the wells with the highest values of predictions  
4.2. Summarize the target volume of reserves in accordance with these predictions  
4.3. Provide findings: suggest a region for oil wells' development and justify the choice. Calculate the profit for the obtained volume of reserves  

### Step 5: Calculate risks and profit for each region
5.1. Use the bootstrapping technique with 1000 samples to find the distribution of profit  
5.2. Find average profit, 95% confidence interval and risk of losses. Loss is negative profit; calculate it as a probability and then express as a percentage  
5.3. Provide findings: suggest a region for development of oil wells and justify the choice  

---

# Data Description

Geological exploration data for the three regions are stored in:

- `geo_data_0.csv`
- `geo_data_1.csv`
- `geo_data_2.csv`

Each dataset includes:

| Column | Description |
|--------|-------------|
| `id` | Unique oil well identifier |
| `f0`, `f1`, `f2` | Three features of points (their specific meaning is unimportant) |
| `product` | Volume of reserves in the oil well (thousand barrels) |

---

# Conditions

- Only linear regression is suitable for model training (the rest are not sufficiently predictable).
- When exploring a region, a study of 500 points is carried out; the top 200 are used for profit calculation.
- Budget for development of 200 oil wells = 100 million USD.
- 1 barrel = $4.5 → 1k barrels = $4,500
- After risk evaluation, keep only the regions with risk of losses < 2.5%.
- Choose the region with the **highest average profit**.

---

# Project Evaluation

What reviewers will look at:

- How did you prepare the data for training?
- Have you followed all the steps of the instructions?
- Have you taken into account all the business conditions?
- What are your findings about the task study?
- Have you applied the **Bootstrapping** technique correctly?
- Have you suggested the best region for well development? Is the choice justified?
- Did you avoid code duplication?
- Have you kept to the project structure and kept the code neat?

---
