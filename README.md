# Customer Segmentation & Data Mining – Food Delivery Platform

## Project Overview

This project focuses on customer segmentation for a food delivery platform, **ABCDEats Inc.**, using customer behavioral, demographic, temporal, cuisine preference, vendor interaction, and spending-related data.

The objective was to identify meaningful customer groups and translate the clustering results into actionable business strategies for targeted marketing, loyalty programs, customer engagement, and operational improvement.

This project was developed as part of the **Data Mining** coursework at **NOVA IMS – Information Management School, Lisbon**.

---

## Business Problem

Food delivery customers differ in how often they order, when they order, how much they spend, which cuisines they prefer, and how they interact with vendors. Treating all customers the same can lead to inefficient promotions and missed business opportunities.

This project answers the question:

> How can customer data be used to identify distinct customer segments and support data-driven marketing strategies?

The segmentation results can help the platform design more effective actions such as:

- Targeted promotions
- Personalized offers
- Loyalty and retention programs
- Cuisine-based recommendations
- Customer engagement strategies
- Vendor and operational planning

---

## Dataset Description

The dataset contains customer-level information collected over a three-month period from a food delivery platform.

The original dataset includes:

- **31,888 customer records**
- **56 features**
- Customer demographic attributes
- Ordering behavior
- Vendor interaction metrics
- Cuisine preferences
- Temporal ordering patterns
- Spending and expenditure-related attributes

Examples of features used in the analysis include:

- `customer_age`
- `customer_region`
- `vendor_count`
- `product_count`
- `is_chain`
- `first_order`
- `last_order`
- Day-of-week order behavior
- Hour-of-day order behavior
- Cuisine categories
- Total amount spent
- Order frequency
- Average vendor usage

---

## Project Workflow

The project followed a full data mining workflow:

1. Data understanding
2. Missing value analysis
3. Outlier detection and treatment
4. Feature engineering
5. Data scaling
6. Feature grouping by perspective
7. K-Means clustering
8. Hierarchical clustering
9. Cluster evaluation
10. Cluster profiling
11. Business insight generation

---

## Data Understanding

Initial exploratory analysis was used to understand customer behavior, ordering patterns, cuisine preferences, and platform engagement.

Some important observations included:

- The customer base was relatively young, with an average age of approximately **27.5 years**
- Customers placed their first order around **28.5 days** into the observed timeline on average
- The average gap between first and most recent order was approximately **63.7 days**
- Ordering behavior varied by weekday, weekend, and time of day
- Cuisine preferences showed clear differences across customer groups
- Spending and vendor interaction patterns were important indicators for customer segmentation

These findings helped guide the feature engineering and clustering strategy.

---

## Data Treatment

### Missing Values

Missing values were analyzed across the dataset. Since the dataset was largely complete, selected missing values were treated using appropriate imputation methods.

### Outlier Handling

Outliers were handled carefully to preserve meaningful customer behavior while reducing extreme noise.

The project explored and applied techniques such as:

- Visual inspection
- Manual thresholding
- IQR-based outlier detection
- Domain-based filtering
- Capping extreme values where appropriate

This helped improve clustering quality and reduce distortion from extreme observations.

---

## Feature Engineering

Feature engineering was a major part of the project. Raw customer data was transformed into structured variables that better represented customer behavior and preferences.

Engineered features included:

- Orders in the morning
- Orders in the afternoon
- Orders at night
- Total number of orders
- Order frequency
- Average vendor usage
- Customer age group
- Cuisine spending categories
- Cuisine preference ratios
- Vendor interaction indicators

Cuisine-related variables were grouped into broader categories, including:

- American cuisine
- Asian cuisine
- European cuisine
- Snacks and beverages
- Other cuisines

These engineered features allowed the segmentation to capture customer behavior from multiple perspectives.

---

## Feature Perspectives

To create more meaningful customer profiles, the clustering analysis was performed from several perspectives.

### 1. Behaviour Perspective

This perspective focused on how customers use the platform, including order frequency, order timing, weekend or weekday activity, product count, vendor count, and average vendor usage.

### 2. Food Preference Perspective

This perspective focused on cuisine preferences and food-related behavior, including American, Asian, European, snacks and beverages, and other cuisine categories.

### 3. Order Perspective

This perspective emphasized ordering patterns such as order count, timing of orders, order frequency, vendor count, and product count.

### 4. Expenditure Perspective

This perspective focused on customer spending behavior, including total amount spent, cuisine-specific expenditure, spending ratios, and order-related monetary behavior.

### 5. Combined Perspective

The final segmentation combined behavioral, food preference, order, expenditure, and vendor interaction features to create a more complete customer profile.

---

## Clustering Methods

The project applied and compared clustering techniques including:

- **K-Means Clustering**
- **Hierarchical Clustering**
- Ward’s linkage method
- Euclidean distance
- Elbow method
- Silhouette score analysis
- Correlation-based feature reduction
- Cluster centroid analysis

The final clustering solution was selected based on both quantitative evaluation and business interpretability.

---

## Final Clustering Profiles

The final analysis produced customer clusters from multiple perspectives.

### Behaviour Perspective

The behaviour-based segmentation identified differences in platform usage, order timing, product variety, vendor interaction, and engagement intensity.

The final behaviour perspective produced multiple clusters with different customer activity levels, including customers with high activity, moderate behavior, and lower engagement.

### Food Preference Perspective

The food preference segmentation showed that cuisine choices were important in differentiating customer groups.

Some customers showed stronger preferences for specific cuisine categories, while others had broader and more balanced food preferences.

### Order Perspective

The order perspective highlighted differences in ordering frequency, time-based ordering patterns, and customer activity levels.

This helped identify groups such as frequent orderers, occasional users, and customers with specific ordering-time behavior.

### Expenditure Perspective

The expenditure perspective showed how customers differ in spending behavior.

Some groups had higher spending intensity, while others appeared more conservative or promotion-sensitive.

### Combined Perspective

The combined perspective integrated all key feature groups and produced the final business-oriented customer segmentation.

This final segmentation was used to generate customer profiles and strategic recommendations.

---

## Final Customer Segments

The final combined segmentation identified five main customer groups:

| Cluster | Segment Name | Description | Recommended Business Action |
|---|---|---|---|
| Cluster 0 | Balanced Customers | Customers with moderate spending patterns and steady ordering behavior. They show balanced activity across different features. | Focus on consistent engagement through stable offers and traditional menu options. |
| Cluster 1 | High-Value Explorers | High-value customers with diverse preferences and frequent orders. They show high spending and willingness to explore premium options. | Offer loyalty programs, upselling opportunities, exclusive deals, and premium offers. |
| Cluster 2 | Conservative Routine-Oriented Customers | Customers who prefer familiar cuisines and show lower spending habits. They are more consistent but less exploratory. | Maintain affordability, reliability, and familiar options to sustain engagement. |
| Cluster 3 | Consistent Spenders | Customers with moderate spending across a mix of cuisines and steady purchase behavior. | Use standard offers, periodic promotions, and personalized engagement campaigns. |
| Cluster 4 | Bargain Hunters | Customers responsive to discounts, affordable offerings, and promotional options. | Provide promotional campaigns, low-cost bundles, and discount-based retention strategies. |

---

## Key Insights

The analysis showed that:

- Customer behavior varies significantly across ordering, cuisine, vendor, and spending dimensions
- High-value customers tend to show broader preferences and stronger engagement
- Some customers are more routine-oriented and prefer familiar or affordable options
- Spending behavior and cuisine preference are important drivers of segmentation
- Combining multiple perspectives produces stronger customer profiles than using a single feature group
- Customer segmentation can support more targeted and effective business strategies

---

## Business Value

The project provides practical value for a food delivery platform by supporting:

- Customer targeting
- Personalized marketing
- Loyalty program development
- Promotion strategy design
- Customer retention planning
- Cuisine recommendation improvement
- Vendor and operational decision-making

Instead of applying one general strategy to all users, the business can design different actions for different customer groups.

---

## Repository Structure

```text
.
├── DM2425_Part2_03(Report).pdf
├── DM2425_Part2_03_01.ipynb
├── DM2425_Part2_03_02.ipynb
└── README.md
