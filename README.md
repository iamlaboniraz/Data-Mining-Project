# Customer Segmentation & Data Mining – Food Delivery Platform

## Project Overview

This project focuses on customer segmentation for a food delivery platform using real-world transactional and behavioral data. The goal is to identify meaningful customer groups based on ordering behavior, spending patterns, cuisine preferences, vendor interactions, and engagement characteristics.

Customer segmentation helps businesses better understand their users and design more effective marketing strategies, loyalty programs, personalized recommendations, and customer retention actions.

This project was developed as part of the **Data Mining** coursework at **NOVA IMS, Lisbon**.

---

## Business Problem

Food delivery platforms serve customers with different preferences, habits, and levels of engagement. Treating all users the same can lead to ineffective marketing and missed business opportunities.

The main objective of this project is to answer:

> How can we group customers into meaningful segments using behavioral and transactional data?

By identifying customer segments, the platform can support data-driven decisions such as:

- Targeted promotions
- Personalized offers
- Loyalty program design
- Customer retention strategies
- Vendor and cuisine recommendation improvements

---

## Dataset

The project uses a large-scale food delivery dataset containing:

- **31K+ users**
- **50+ features**
- Customer spending behavior
- Cuisine preferences
- Ordering time patterns
- Vendor interactions
- Transactional and behavioral attributes

The dataset contained noisy real-world data, requiring preprocessing and feature transformation before clustering.

---

## Methodology

The project follows an end-to-end data mining workflow:

1. Data understanding
2. Data cleaning and preprocessing
3. Missing value treatment
4. Outlier handling
5. Feature engineering
6. Feature scaling
7. Correlation-based feature reduction
8. Clustering model development
9. Cluster evaluation
10. Customer profile interpretation
11. Business insight generation

---

## Data Preprocessing

Several preprocessing steps were applied to improve data quality and model reliability:

- Handled missing values through imputation
- Treated outliers to reduce distortion in clustering
- Scaled numerical features for distance-based algorithms
- Transformed raw transactional data into structured customer-level features
- Removed highly correlated or redundant features
- Prepared the final dataset for unsupervised learning

---

## Clustering Techniques

Two clustering approaches were applied and compared:

### K-Means Clustering

K-Means was used to group customers based on numerical behavioral features. The optimal number of clusters was selected using:

- Elbow method
- Silhouette analysis
- Cluster interpretability

### Hierarchical Clustering

Hierarchical clustering was used to explore customer similarity structures and validate segmentation patterns from another clustering perspective.

---

## Final Segmentation

The final segmentation selected **5 customer clusters** based on clustering performance and business interpretability.

Each cluster was analyzed using:

- Cluster centroids
- Spending patterns
- Cuisine preferences
- Ordering behavior
- Vendor engagement
- Customer activity levels

The resulting customer profiles helped translate clustering outputs into business-facing insights.

---

## Key Insights

The segmentation analysis enabled the identification of different customer groups, such as:

- High-value frequent customers
- Price-sensitive or promotion-driven customers
- Low-engagement customers
- Cuisine-specific customers
- Customers with diverse ordering behavior

These insights can help the business design more targeted and effective marketing strategies.

---

## Business Value

The project supports business decision-making by enabling:

- More personalized customer targeting
- Better loyalty and retention strategies
- Improved campaign design
- Data-driven customer profiling
- Better understanding of customer behavior across the platform

Instead of applying one generic strategy to all users, the platform can tailor actions based on customer segment behavior.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure

```text
customer-segmentation-data-mining/
│
├── data/
│   └── README.md
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_preprocessing_feature_engineering.ipynb
│   ├── 03_clustering_modeling.ipynb
│   └── 04_cluster_analysis_business_insights.ipynb
│
├── reports/
│   ├── figures/
│   └── project_report.pdf
│
├── src/
│   ├── preprocessing.py
│   ├── clustering.py
│   └── visualization.py
│
├── requirements.txt
├── README.md
└── .gitignore
