# **Customer Segmentation Analysis for Marketing Strategy**

# 1. Introduction

The objective of this analysis is to develop a customer segmentation strategy based on the usage behavior of credit card holders. The dataset used contains information on approximately 9000 active credit card holders over the last 6 months, focusing on 18 behavioral variables. The segmentation aims to provide insights for targeted marketing strategies, personalized customer experiences, and improved customer retention.


# 2. Dataset

The dataset used for this analysis is called "Credit Card Dataset" and is sourced from Kaggle (https://www.kaggle.com/datasets/arjunbhasin2013/ccdata). It includes the following variables:

CUST_ID: Identification of Credit Card holder (Categorical)

BALANCE: Balance amount left in the account to make purchases

BALANCE_FREQUENCY: Frequency of balance updates (0 = not frequently updated, 1 = frequently updated)

PURCHASES: Amount of purchases made from the account
ONEOFF_PURCHASES: Maximum purchase amount done in one-go

INSTALLMENTS_PURCHASES: Amount of purchase done in installments

CASH_ADVANCE: Cash in advance given by the user
PURCHASES_FREQUENCY: Frequency of purchases being made

ONEOFF_PURCHASES_FREQUENCY: Frequency of one-off purchases

PURCHASES_INSTALLMENTS_FREQUENCY: Frequency of purchases in installments

CASH_ADVANCE_FREQUENCY: Frequency of cash in advance being paid

CASH_ADVANCE_TRX: Number of transactions made with "Cash in Advance"

PURCHASES_TRX: Number of purchase transactions made

CREDIT_LIMIT: Limit of Credit Card for the user

PAYMENTS: Amount of Payment done by user

MINIMUM_PAYMENTS: Minimum amount of payments made by user

PRCFULLPAYMENT: Percent of full payment paid by user

TENURE: Tenure of credit card service for the user

# 3. Methodology

### Data Preprocessing:

Checked for missing values and filled them with the mean value for 'CREDIT_LIMIT' and 'MINIMUM_PAYMENTS'.
Converted categorical variables to numerical using label encoding or one-hot encoding if necessary.
Exploratory Data Analysis:

Created a correlation matrix and heatmap to visualize the correlations between variables.
Identified strong correlations such as 'PURCHASES_TRX' and 'PURCHASES' with a correlation coefficient of 0.69, indicating a strong positive relationship.

### Clustering:

Used the elbow method to determine the optimal number of clusters, which indicated that 8 clusters would be appropriate.
Applied KMeans clustering with 8 clusters to segment the customers based on their behavior.

# 4. Results and Analysis

The clustering analysis revealed distinct customer segments with unique behavioral patterns:

Cluster 0: Low spenders with low frequency of purchases and cash advances.
Cluster 1: High spenders with high credit limits and frequent purchases.
Cluster 2: Moderate spenders with average credit limits and moderate purchase frequency.
Cluster 3: Customers with high cash advances but low purchases.
Cluster 4: Customers with very low activity across all variables.
Cluster 5: Customers with high one-off purchases and low installment purchases.
Cluster 6: Customers with high installment purchases frequency.
Cluster 7: Customers with high full payment percentages and low balance.

# 5. Business Implications

Targeted Marketing: Each cluster represents a different customer segment with unique needs and behaviors. This segmentation can help in creating targeted marketing campaigns tailored to each segment's preferences.

Customer Retention: By understanding customer behavior, strategies can be developed to retain customers by offering personalized experiences and incentives.

Product Development: Insights from the segmentation can guide product development efforts, such as introducing new features or services based on the needs of different customer segments.

# 6. Conclusion

Customer segmentation is a powerful tool for businesses to understand their customers better and tailor their strategies accordingly. By analyzing the credit card dataset and applying clustering techniques, we have identified distinct customer segments with unique behaviors. This segmentation can be used to drive targeted marketing strategies, improve customer retention, and enhance overall customer satisfaction.
