
# Customer Segmentation using K-Means Clustering

## Project Overview

This project performs **customer segmentation** using the K-Means clustering algorithm. Customer segmentation helps businesses group customers based on similar characteristics such as income and spending behavior.

The goal of this project is to identify different customer groups so that businesses can better understand their customers and apply targeted marketing strategies.

---

# Dataset Description

The dataset contains information about customers and their purchasing behavior.

### Features in the Dataset

| Feature        | Description                                          |
| -------------- | ---------------------------------------------------- |
| Customer ID    | Unique identifier for each customer                  |
| Gender         | Gender of the customer                               |
| Age            | Age of the customer                                  |
| Annual Income  | Annual income of the customer                        |
| Spending Score | Score assigned based on customer purchasing behavior |

The **Spending Score** ranges from 1 to 100 and indicates how actively a customer spends.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

# Project Workflow

The following steps were performed in this project:

### 1. Data Loading

The dataset was imported and inspected to understand its structure.

### 2. Data Exploration

Basic analysis was performed using:

* `head()`
* `info()`
* `describe()`
* missing value check

### 3. Data Visualization

Initial visualizations were created to understand customer distribution:

* Age distribution
* Gender distribution

### 4. Feature Selection

The following features were selected for clustering:

* Annual Income
* Spending Score

### 5. Feature Scaling

Data was scaled using **StandardScaler** to improve clustering performance.

### 6. Finding Optimal Clusters

The **Elbow Method** was used to determine the optimal number of clusters.

### 7. K-Means Clustering

The K-Means algorithm was applied to group customers into segments.

### 8. Cluster Visualization

Customer segments were visualized using scatter plots.

### 9. Cluster Analysis

Cluster averages were calculated to understand the characteristics of each segment.

---

# Results

The analysis identified **five distinct customer segments** based on income and spending behavior.

These segments include:

* High income – high spending customers
* High income – low spending customers
* Low income – low spending customers
* Moderate income – moderate spending customers
* Low income – relatively higher spending customers

This segmentation helps businesses understand different types of customers.

---

# Visualizations Included

The project includes the following visualizations:

* Age distribution
* Gender distribution
* Elbow method graph
* Customer segmentation scatter plot
* Cluster distribution plot

---

# Project Structure

```
Customer-Segmentation
│
├── customer_segmentation.ipynb
├── Mall_Customers.csv
├── Customer_Segmentation_Report.pdf
└── README.md
```

---

# Key Insights

* Customers can be grouped into distinct segments based on their purchasing behavior.
* Some customers show high spending patterns and are valuable to the business.
* Certain customers have high income but low spending potential.
* Businesses can use these insights for targeted marketing strategies.

---

# Conclusion

Customer segmentation using K-Means clustering helps identify patterns in customer behavior. This allows businesses to better understand their customers and improve marketing strategies.

This project demonstrates how clustering techniques can be used in data science to solve real-world business problems.

---


