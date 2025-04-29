# Project of Supervised Learning

## Project Description

Beta Bank is facing a problem: customers are leaving the service gradually. Management believes that it is cheaper to retain existing customers than to acquire new ones. Your mission is to predict whether a customer will soon leave the bank using historical customer behavior data.

You have access to past banking activity and termination records. Your goal is to develop a classification model that predicts churn with the **highest possible F1 score**. To pass the project, the F1 score on the test set must be **at least 0.59**.

In addition, you must evaluate the **AUC-ROC** metric and compare it with the F1 score.

---

## Project Instructions

1. **Download and prepare the data.** Explain how you did it.
2. **Explore class imbalance.** Train a baseline model without balancing the classes and describe the results.
3. **Improve the model using at least two techniques for dealing with imbalance.** Use training and validation sets to tune and compare multiple models.
4. **Perform final testing** on the best model.

---

## Data Description

The dataset is located at `/datasets/Churn.csv` and contains the following features:

### Features

- `RowNumber` – data string index  
- `CustomerId` – unique customer identifier  
- `Surname` – customer surname  
- `CreditScore` – credit score  
- `Geography` – country of residence  
- `Gender` – gender  
- `Age` – age  
- `Tenure` – how long the customer has stayed with the bank  
- `Balance` – account balance  
- `NumOfProducts` – number of bank products used  
- `HasCrCard` – has a credit card (0/1)  
- `IsActiveMember` – active membership (0/1)  
- `EstimatedSalary` – estimated salary  

### Target

- `Exited` – whether the customer left the bank (1) or not (0)

---

## Evaluation Criteria

The project will be evaluated on the following:

- Have you prepared the data and processed the feature types correctly?
- Have you clearly explained the preprocessing steps?
- Did you investigate the **class balance**?
- Did you evaluate an **unbalanced baseline model**?
- What approaches did you try for balancing (e.g., class weighting, oversampling, undersampling)?
- Have you correctly split the data into **training, validation, and test sets**?
- Did you use at least **two different imbalance-handling techniques**?
- Did you run proper training, validation, and **final testing**?
- What was your final **F1 score**?
- Did you compare the **AUC-ROC** to the F1 score?
- Is your code **structured**, **clean**, and well-commented?

---
=======
# Project 9
>>>>>>> f472bd4 (Initial commit)
