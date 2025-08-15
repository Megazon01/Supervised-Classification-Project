# California Housing Location Classification

## 📌 Project Overview
This project uses **supervised machine learning** to classify whether a house in California is **close** or **far** from the ocean based on two key features:
- Median household income
- Median house value

The dataset originates from the [California Housing dataset](https://raw.githubusercontent.com/ageron/handson-ml/master/datasets/housing/housing.csv), which contains demographic, economic, and geographical information about housing in California.

## 🎯 Objective
The goal is to train and evaluate a classification model that predicts ocean proximity from selected numerical features.

## 📂 Dataset Details
- **Source:** [Hands-On Machine Learning with Scikit-Learn & TensorFlow by Aurélien Géron](https://github.com/ageron/handson-ml)
- **Rows:** 20,640
- **Columns:** 10 (including target variable `ocean_proximity`)
- **Target Variable:** `ocean_proximity_bin` (binary: `close` or `far`)

## 🛠 Methodology
1. **Data Preparation**
   - Loaded CSV data directly from an online source using `pandas`
   - Cleaned and transformed categorical target variable (`ocean_proximity`) into binary form (`close`, `far`)
   - Selected relevant features: `median_income` and `median_house_value`
2. **Modeling**
   - Used `train_test_split` to create training and testing sets (75/25 split)
   - Trained a **Logistic Regression** classifier using scikit-learn
3. **Evaluation**
   - Evaluated the model using **accuracy score** and **confusion matrix**
   - Achieved accuracy: **83%**
4. **Interpretation**
   - Analyzed true/false positives and negatives for classification performance

## 📊 Results
Confusion Matrix Example:
 [[3120, 389],
 [ 494, 1156]]

- **True Close:** 3120  
- **True Far:** 1156  

### 📎 Requirements

Dependencies are listed in requirements.txt and include:
* pandas
* numpy
* scikit-learn
* matplotlib

### 📜 License 

This project is for educational purposes and uses publicly available data.
