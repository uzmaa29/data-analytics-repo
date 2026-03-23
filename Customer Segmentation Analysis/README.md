# Customer Segmentation Analysis using K-Means Clustering

## 1. Introduction

Customer segmentation is an important technique used by businesses to divide customers into groups based on similar characteristics or purchasing behavior. By understanding different customer segments, companies can design better marketing strategies, improve customer satisfaction, and increase overall sales.

In this project, customer segmentation is performed using the **K-Means clustering algorithm**. The dataset contains information about customers such as age, gender, annual income, and spending score. The objective of this analysis is to identify distinct customer groups based on their income and spending behavior.

---

## 2. Dataset Description

The dataset contains information about customers and their purchasing behavior. Each record represents a single customer.

The dataset includes the following features:

| Column         | Description                                 |
| -------------- | ------------------------------------------- |
| Customer ID    | Unique identifier for each customer         |
| Gender         | Gender of the customer                      |
| Age            | Age of the customer                         |
| Annual Income  | Annual income of the customer               |
| Spending Score | Score assigned based on purchasing behavior |

The **Spending Score** ranges from 1 to 100 and represents how actively a customer spends in the store.

---

## 3. Data Exploration

Initially, the dataset was explored to understand its structure and characteristics.

The following steps were performed:

* Displayed the first few rows of the dataset using `df.head()`
* Checked dataset information using `df.info()`
* Generated summary statistics using `df.describe()`
* Checked for missing values using `df.isna().sum()`

The dataset did not contain missing values, making it suitable for analysis.

---

## 4. Data Visualization

Basic visualizations were created to better understand customer demographics.

### Age Distribution

A histogram was used to analyze the distribution of customer ages. This helped identify the age groups that make up the majority of customers.

### Gender Distribution

A count plot was used to observe the number of male and female customers in the dataset.

These visualizations provide a better understanding of the dataset before applying clustering techniques.

---

## 5. Feature Selection

For customer segmentation, the following features were selected:

* Annual Income
* Spending Score

These features are important because they directly reflect a customer's purchasing power and buying behavior.

---

## 6. Feature Scaling

Before applying the clustering algorithm, feature scaling was performed using **StandardScaler**. Scaling ensures that all features contribute equally to the clustering process and prevents bias caused by differences in magnitude.

---

## 7. Determining the Optimal Number of Clusters

The **Elbow Method** was used to determine the optimal number of clusters.

In this method, the inertia value is calculated for different numbers of clusters, and the results are plotted on a graph. The point where the graph begins to bend (the elbow point) indicates the optimal number of clusters.

From the graph, the optimal number of clusters was determined to be **5**.

---

## 8. K-Means Clustering

After determining the optimal number of clusters, the **K-Means algorithm** was applied to the dataset.

Each customer was assigned to one of the five clusters based on their income and spending behavior.

This step allowed the identification of different customer segments.

---

## 9. Customer Segmentation Visualization

A scatter plot was used to visualize the customer segments based on:

* Annual Income (x-axis)
* Spending Score (y-axis)

Each cluster was represented by a different color. This visualization clearly showed how customers are grouped into distinct segments.

Another visualization was created to show the **number of customers in each cluster**.

---

## 10. Cluster Analysis

The average values of each cluster were calculated to better understand customer characteristics.

The clusters can be interpreted as follows:

Cluster 0: Customers with moderate income and moderate spending behavior.

Cluster 1: Customers with high income and high spending score. These customers are considered premium customers and are very valuable to the business.

Cluster 2: Customers with low income and low spending score. These customers are less active in purchasing.

Cluster 3: Customers with high income but low spending score. These customers have potential and can be targeted through marketing strategies.

Cluster 4: Customers with low income but relatively higher spending score compared to others.

These clusters help businesses understand customer behavior and design targeted marketing campaigns.

---

## 11. Key Insights

The analysis provided several important insights:

* Customers can be divided into distinct groups based on income and spending behavior.
* A group of customers shows high income and high spending patterns, making them the most valuable segment.
* Some customers have high income but low spending, indicating potential for targeted promotions.
* Low-income customers generally have lower spending scores.

Customer segmentation helps businesses focus on the right group of customers for different marketing strategies.

---

## 12. Business Recommendations

Based on the analysis, the following recommendations can be made:

* Provide loyalty programs and exclusive offers for high-spending customers.
* Encourage high-income customers with low spending scores through personalized promotions.
* Offer discounts or affordable products to attract low-income customers.
* Use targeted marketing campaigns for each customer segment.

---

## 13. Conclusion

This project successfully applied the **K-Means clustering algorithm** to perform customer segmentation. The analysis revealed distinct groups of customers based on their income and spending behavior.

Customer segmentation is an effective approach that helps businesses understand customer needs and improve decision-making. By targeting different customer groups with appropriate strategies, companies can enhance customer engagement and increase profitability.

