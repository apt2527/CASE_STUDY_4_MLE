
DATASET LINK: https://www.archive.ics.uci.edu/dataset/502/online%2Bretail%2Bii?utm_source=chatgpt.com


# Customer Segmentation Using RFM Analysis and K-Means Clustering

## Project Overview

Customer Segmentation is a data analysis and machine learning project that groups customers based on their purchasing behaviour.

This project uses the Online Retail II dataset to analyze customer transactions and identify meaningful customer segments using RFM Analysis and K-Means Clustering.

The objective is to help businesses understand customer purchasing patterns, identify valuable customer groups, and develop targeted marketing strategies.

## Objectives

* Analyze customer purchasing behaviour.
* Calculate Recency, Frequency, and Monetary (RFM) values.
* Apply data preprocessing and feature scaling.
* Segment customers using the K-Means clustering algorithm.
* Evaluate clustering results using the Elbow Method and Silhouette Score.
* Visualize customer segments using Principal Component Analysis (PCA).
* Assign customer personas and recommend marketing strategies.

## Dataset

**Dataset Name:** Online Retail II

**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

The dataset contains transaction records from a UK-based online retail business covering December 2009 to December 2011.

### Dataset Features

| Feature     | Description                      |
| ----------- | -------------------------------- |
| Invoice     | Invoice or transaction number    |
| StockCode   | Product identification code      |
| Description | Product description              |
| Quantity    | Number of products purchased     |
| InvoiceDate | Date and time of the transaction |
| Price       | Price per item                   |
| Customer ID | Customer identification number   |
| Country     | Customer's country               |

The original dataset contains approximately 1.07 million transaction records. The number of records used in the analysis depends on data cleaning and preprocessing.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook
* Google Colab

## Project Workflow

### 1. Data Loading and Cleaning

* Load the retail dataset.
* Handle missing values.
* Remove duplicate records.
* Convert transaction dates into datetime format.
* Calculate transaction values.

### 2. RFM Analysis

RFM analysis summarizes customer purchasing behaviour using three metrics:

* **Recency:** Number of days since the customer's last purchase.
* **Frequency:** Number of unique invoices associated with the customer.
* **Monetary:** Total transaction value associated with the customer.

These metrics transform transaction-level data into customer-level features.

### 3. Feature Engineering and Scaling

* Select the RFM features.
* Apply log transformation to reduce skewness.
* Standardize the features using StandardScaler.
* Prepare the data for clustering.

### 4. K-Means Clustering

K-Means is an unsupervised machine learning algorithm that groups customers based on the similarity of their RFM characteristics.

The project evaluates different cluster counts using:

* **Elbow Method:** Examines changes in within-cluster inertia.
* **Silhouette Score:** Measures how well-separated the clusters are.

The selected number of clusters is then used to train the final model.

### 5. PCA Visualization

Principal Component Analysis (PCA) reduces the three-dimensional RFM feature representation to two principal components.

This allows customer clusters to be visualized in a two-dimensional scatter plot.

PCA is used for visualization, while K-Means performs clustering using the scaled RFM features.

### 6. Customer Profiling and Personas

The resulting clusters are summarized using average Recency, Frequency, and Monetary values.

Based on the


