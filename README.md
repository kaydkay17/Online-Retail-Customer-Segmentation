# Customer-Segmentation

## Problem Statement:
In this project, your task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

## Attribute Information:
* InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
* StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
* Description: Product (item) name. Nominal.
* Quantity: The quantities of each product (item) per transaction. Numeric.
* InvoiceDate: Invice Date and time. Numeric, the day and time when each transaction was generated.
* UnitPrice: Unit price. Numeric, Product price per unit in sterling.
* CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
* Country: Country name. Nominal, the name of the country where each customer resides.


## Summary:
In this project, our task was to identify major customer segments on a transnational data set that contained one-year historical transactions for a UK-based online retail store. This would help the company segregate its customers based on transaction data and help them in marketing decisions and strategy.

After basic exploration and cleaning the data we found relationships between features in EDA and then jumped into the analysis part. Cohort analysis helped us understand the customer retention rate and revenue retention rate for the company. Then based on the given features like unit price, quantity, purchase date, etc. we extracted RFM values, RFM scores for store customers. 

After transforming and scaling the features we developed a clustering model using K-means to find major customer segments. In order to achieve the optimal number of clusters we used the elbow criterion, Silhouette score and also implemented Agglomerative clustering with the help of Dendrogram.
Based on the results and the store’s requirements we successfully segmented customers into 3 clusters according to their shared characteristics.
