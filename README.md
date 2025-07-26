# 🛍️ Customer Segmentation using KMeans Clustering

This project implements customer segmentation using K-Means clustering on retail store customer data to group customers based on purchasing behavior (Annual Income and Spending Score).

## 📌 Table of Contents
- [Task Objective](#-task-objective)
- [Features](#-features)
- [Dataset](#-dataset)
- [Workflow](#-workflow)
- [Methodology](#-methodology)
- [Results](#-results)
- [Getting Started](#-getting-started)

## 🎯 Task Objective
Group similar customers together for targeted marketing based on:
- 🎂 Age
- 💸 Annual Income (k$)
- 💳 Spending Score (1-100)

## 🔧 Features
- Data cleaning and preprocessing
- Label encoding for categorical values
- Feature selection and engineering
- Elbow method to find optimal clusters
- KMeans clustering and analysis
- Multiple visualizations:
  - 📉 Elbow Method Plot
  - 📊 Cluster Visualizations
  - 🎯 Gender & Age distribution across clusters
  - 🔄 Pairwise Feature Relationships

## 📂 Dataset
**Source:** [Mall Customer Segmentation Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) 

## 🛠️ Workflow
1. **Data Preprocessing** 🔧
   - Renamed columns for clarity
   - Encoded Gender to numeric
   - Handled missing values (if any)

2. **Clustering Preparation** 🧮
   - Selected features: Age, Annual Income, Spending Score
   - Scaled values (optional)
   - Determined K using the Elbow Method

3. **Model Training** 🤖
   - Applied KMeans(n_clusters=5)
   - Assigned cluster labels to data

4. **Evaluation** 📊
   - No external accuracy/loss (unsupervised learning)
   - Cluster analysis using visuals and group statistics

## 🧠 Methodology
1. **Data Preprocessing & Cleaning** 🧹  
   Handled missing values and standardized column names.

2. **Label Encoding** 🔢  
   Converted categorical variables like Gender into numerical format.

3. **Feature Selection** 🎯  
   Selected features: Age, Annual Income, and Spending Score.

4. **Elbow Method** 🔍  
   Determined optimal number of clusters (K=5) using the Elbow Curve.

5. **KMeans Clustering** 🔄  
   Applied KMeans to segment customers into meaningful groups.

6. **Cluster Analysis** 🏷️  
   Added cluster labels to dataset and visualized patterns.

## 🔍 Clustering Evaluation
| Metric               | Description                          |
|----------------------|--------------------------------------|
| Inertia              | Printed from Elbow Method            |
| Silhouette Score     | Measures how well-clustered the data |


## ✅ Results
### 📋 Cluster Summary (Means)
| Cluster | Age (Mean) | Income (Mean) | Spending Score (Mean) |
|---------|------------|---------------|-----------------------|
| 0       | 25.3       | 25.4          | 80.2                  |
| 1       | 45.7       | 78.5          | 18.7                  |
| 2       | 32.1       | 55.1          | 55.5                  |
| 3       | 27.9       | 60.3          | 35.2                  |
| 4       | 40.8       | 88.6          | 90.1                  |


## 🚀 Getting Started
1. Clone the repository
```bash
git clone https://github.com/suman2896/SCT_ML_2.git
cd mall-customer-segmentation
