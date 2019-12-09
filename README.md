# Datathon_IE_university
The following project is the result of a datathon competition based on a dataset presenting 14 different features for 2018 listings on the **hotelbeds.com** platform.

The target for this model is to find pricing anomalies among the roughly 900,000 listings provided. 

### Approach Abstract

Detecting outliers or anomalies in pricing from the bookings data is an unsupervised learning problem. The problem is approached with a three-pronged flow:

#### 1. Tag Explicit Errors and Meaningless Values
#### 2. Remove extreme values contrary to domain standards
##### 2.1. Check for statistical outliers based on calculated Outlier Score
#### 3. Cluster similar bookings based on pricipal components and detect statistical outliers



------------------------------------------------------------------------------------------------------------------------



The group proceeded with the above approach while forming 2 basic assumptions/hypothesis:

#### 1. Clusters or features that have higher standard deviations, kurtosis or extreme values are more likely to contain anomalies
#### 2. Total anomalies will probably not be higher than 1% of the data set


The above approach is implemented by exploring the dataset and creating sub-sets of the data  that are likely to be anomalies at each level. In the end these subsets of data are combined to create the prediction .csv with the final tag = 1 for anomalies, 0 for genuine.

### End Result
The end result shows the following number of pricing anomalies according to each step of model:

**Meaningless values:** 8820

**Extreme Values:** 112

**Outlier Score:** 123

**Price Regression:** 708

**TOTAL: 9763 (10.85% of the original dataset)

