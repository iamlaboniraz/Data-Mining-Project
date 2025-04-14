# Introduction :
In today’s competitive landscape of food delivery services, understanding customer preferences is pivotal to success. ABCDEats. Inc, a dynamic food delivery platform, recognizes this challenge and embarks on a data-driven journey to enhance its customer segmentation strategy. By leveraging 
customer data collected over three months from three distinct cities, the company seeks to uncover meaningful patterns and insights that will enable personalized services and targeted marketing campaigns.The goal is to identify diverse customer segments by analyzing attributes such as purchasing behavior, demographic information, and culinary preferences. These insights will empower ABCDEats to tailor its offerings to better meet the needs and preferences of each customer
group, ultimately fostering stronger customer engagement, satisfaction, and loyalty. This project involves a comprehensive exploration of the dataset, identification of key variables for segmentation, and the application of clustering techniques to delineate customer groups. Each segment will be
thoroughly analyzed to highlight its unique characteristics, ensuring that the final segmentation strategy is not only data-informed but also aligned with ABCDEats' broader business objectives.By integrating Culinary-based, Behaviour-based, and Expenditure perspectives into the segmentation framework, ABCDEats aims to craft a holistic marketing strategy that resonates with its diverse customer base. This endeavor not only positions the company to optimize its operations but also paves the way for sustainable growth in the ever-evolving food delivery market.

## Dataset Description
The dataset provided for this project includes customer data from ABCDEats Inc. and consists of multiple
columns capturing various customer attributes and aggregating their behaviour over a three-month period.
Each row corresponds to one customer, and the column descriptions are given below:
# Column Name Description
1 customer_id Unique identifier for each customer.
2 customer_region Geographic region where the customer is located.
3 customer_age Age of the customer.
4 vendor_count Number of unique vendors the customer has ordered from.
5 product_count Total number of products the customer has ordered.
6 is_chain Indicates whether the customer’s order was from a chain restaurant.
7 first_order Number of days from the start of the dataset when the customer first placed an order.
8 last_order Number of days from the start of the dataset when the customer most recently placed an order.
9 last_promo The category of the promotion or discount most recently used by the customer.
10 payment_method Method most recently used by the customer to pay for their orders.
11 CUI_American, CUI_Asian, CUI_Chinese, CUI_Italian, etc.
The amount in monetary units spent by the customer from the indicated type of cuisine.
12 DOW_0 to DOW_6 Number of orders placed on each day of the week (0 = Sunday, 6 = Saturday).
13 HR_0 to HR_23 Number of orders placed during each hour of the day (0 = midnight, 23 = 11 PM).
