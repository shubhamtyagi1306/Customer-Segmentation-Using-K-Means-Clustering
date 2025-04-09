# 🛍️ Customer Segmentation Using K-Means Clustering

## 📌 Project Overview

This project applies **K-Means Clustering**, an unsupervised machine learning algorithm, to segment mall customers based on their **Annual Income** and **Spending Score**. The goal is to identify distinct customer groups to help businesses make data-driven marketing decisions.

---

## 📂 Dataset

**Source:** [Mall Customer Segmentation Dataset (Kaggle)](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

The dataset contains the following fields:

- `CustomerID`: Unique identifier for each customer
- `Gender`: Male/Female
- `Age`: Age of the customer
- `Annual Income (k$)`: Customer's income in thousands
- `Spending Score (1-100)`: Score assigned by the mall based on spending behavior

---

## 🎯 Objective

- Perform exploratory data analysis (EDA)
- Preprocess and prepare data for clustering
- Determine optimal number of clusters using the Elbow Method
- Apply **K-Means Clustering** to group similar customers
- Visualize and interpret customer segments
- Generate insights to aid business strategy

---

## 🧰 Tools & Technologies

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 🔍 Exploratory Data Analysis (EDA)

- The dataset is clean with no missing values
- Age ranges from **18 to 70 years**
- Annual income ranges from **$15k to $137k**
- Spending score ranges from **1 to 99**

### Distribution Plots:

- **Age** is mostly centered around 30-40 years
- **Annual Income** has a roughly uniform distribution
- **Spending Score** is more concentrated in the middle range (40–60)

---

## 📈 Finding Optimal Clusters – Elbow Method

Using the **Elbow Method**, we calculated the Within-Cluster-Sum-of-Squares (WCSS) for clusters ranging from 1 to 10. The "elbow" in the graph appeared at **5 clusters**, which is selected as the optimal value for K.

---

## 📊 Clustering Results

The clustering was applied to two features:
- `Annual Income`
- `Spending Score`

### 📌 Cluster Summary:

| Cluster | Characteristics                              | Insights                                 |
|---------|----------------------------------------------|------------------------------------------|
| 0       | High income, high spending                   | 🟢 Target for premium loyalty programs    |
| 1       | Low income, low spending                     | 🔴 Not ideal for high-end promotions     |
| 2       | High income, low spending                    | 🟡 Upsell opportunities with discounts   |
| 3       | Average income, high spending                | 🔵 Engage via regular promotions         |
| 4       | Young, low income, moderate spending         | 🟣 Potential long-term loyal customers   |

---


## ✅ Conclusion

K-Means Clustering proved effective in segmenting customers based on income and spending behavior. These segments can guide:
- Targeted marketing campaigns
- Loyalty reward programs
- Personalized recommendations

---

