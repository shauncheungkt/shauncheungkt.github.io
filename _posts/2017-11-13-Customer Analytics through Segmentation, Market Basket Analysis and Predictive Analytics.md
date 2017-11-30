---
layout: post
title: Customer analytics through RFM segmentation, market basket analysis and predicting behaviour
tags: [customer analytics]
comments: true
---



Customers are more empowered and connected to information than ever before, making customer analytics a necessity to deliver value to customers. 

This Project examines a year of online transaction data from an online retail store with the goal of providing insights to increase effectiveness of marketing and sales effort to customers.


### Project breakdown

1. RFM based customer segmentation using k-means clustering      
<!-- ![Alt text](/images/segmentation.png) to insert picture -->

2. Market basket analysis on each segment to identify purchasing pattern using association rule

3. Predicting customers' behaviour using Lifetimes Python library


<br>

### The data set

This is a transactional data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers. It can be downloaded from: archive.ics.uci.edu/ml/datasets/Online+Retail

```python
online_sales = pd.read_csv("../project-capstone/Online_Retail.csv", parse_dates=True)

online_sales.shape

(541909, 8)

online_sales.head()

 InvoiceNo StockCode  Description	                        	
0 536365	85123A  WHITE HANGING HEART T-LIGHT 	         
1 536365	71053  WHITE METAL LANTERN	                        
2 536365	84406B  CREAM CUPID HEARTS COAT HANGER	           
3 536365	84029G  KNITTED UNION FLAG HOT WATER
4 536365	84029E	RED WOOLLY HOTTIE WHITE HEART	         

Quantity InvoiceDate UnitPrice CustomerID Country
  6  12/1/2010 8:26  2.55	  17850.0	 United Kingdom
  6  12/1/2010 8:26  3.39	  17850.0	 United Kingdom
  8  12/1/2010 8:26  2.75	  17850.0	 United Kingdom
  6  12/1/2010 8:26  3.39	  17850.0	 United Kingdom
  6  12/1/2010 8:26  3.39	  17850.0	 United Kingdom

```
<br><br>
