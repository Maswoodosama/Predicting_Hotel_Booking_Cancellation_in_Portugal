# About the Project
This project aims to predict whether a hotel booking will be **cancelled or not** based on historical booking data from hotels in **portugal 

The goal is to help hotels **reduce revenue loss** and **improve resource planning** by anticipating cancellations using **machine learning models**

## Dataset


**Source:** [Hotel Booking Demand Dataset(ScienceDirect)](https://www.sciencedirect.com/science/article/pii/S2352340918315191)

** Description:**
The dataset contains booking details such as :
- Type of hotel (city or resort)
- lead time
- Number of guests
- Market segment
- special requests
- Previous cancellations
- Deposite type
- Average Daily rate (ADR)
- And more...

**Target Variable:**

'is_canceled'
'1': Booking Canceled
'0': Booking not canceled

## Problem statement
Hotel cancellations have been increasing year after year, causing:
- **Revenue loss**
- **Operational inefficiencies**
- **Inventory mismanagement**

  This project predicts whether a booking will be canceled using machine learning to assist hotel management in proactive decision-making.

  ## Machine Learning Workflow

  ### 1, Data preprocessing
  - Handle missing values and duplicates
  - converted categorical features into numeric using **Label Encoding**
  - Performed feature scaling
  - Conduct **Exploratory Data Analysis (EDA)** to identify cancellation patterns
 
  ### 2, Exploratory Data Analysis (EDA)
  Analyzed relationships between:
  - Lead time and cancellations
  - Deposite type and cancellation probability
  - customer type and hotel type
  - Market segment and average daily rate
 
  Visualized using **Matplotlib** and **Seaborn**

  ### 3, Model Building
  Tested multiple classification algorithms:
  - Logistic Regression
  - Random forest
  - Decision Tree
 
**Evaluation Metrics**
- Accuracy
- Precision
- Recall
- F1-score
- confusion matrix

### 4, Model Selection
selected the model with best balance between and accuracy to minimize false negatives (i,e, booking predicted as "not canceled" but actually canceled)

### Results:
- Best Model: **Random Forest Classifier**
- Accuracy: ~85-90% (depending on hyperparameters)
- The model effectively identified key features affecting cancellations, such as:
- lead time
- Deposite time
- previous cancellations
- Market segment

## Technology used:
**Python**
**Numpy**, **Pandas**
**Matplotlib**, **Seaborn**
**Scikit-learn**

## Insights
- Booking with **long lead times** have higher cancellation rates.
-  **No-deposite bookings** are more likely to be canceled
-  Guests with **previous cancellations** have a higher probability of cancelling again.
-  **City hotels** experience slightly higher cancellations compared to **resort hotels**


**Author**
**Osama Maswood**
