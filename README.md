# datathon_IE_university
The following project is the result of a datathon competition based on a dataset presenting 14 different features for 2018 listings on the **hotelbeds.com** platform.

The target for this model is to find pricing anomalies among the roughly 900,000 listings provided. 

# Approach Abstract

Detecting outliers or anomalies in pricing from the bookings data is an unsupervised learning problem. The problem is approached with a three-pronged flow:

## 1. Tag Explicit Errors and Meaningless Values
## 2. Remove extreme values contrary to domain standards
## 2.1. Check for statistical outliers based on calculated Outlier Score
## 3. Cluster similar bookings based on pricipal components and detect statistical outliers
