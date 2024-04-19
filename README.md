# Spar-Nord-Bank-ETL-Pipeline
**PROBLEM STATEMENT**

Banks have to make sure that they come up with the right strategy to make sure the ATM's are refilled timely and money is not sitting idle either. Cash refilling into ATM's  depends on the activity and the area where a particular ATM is located as well as the weather, day of the week, etc.

Spar Nord Bank is trying to observe the withdrawal bahaviour  and corresponding dependent factors to optimally manage the refill frequency .Spar Nord Bank has also built a dimensional model datastore (ATM Data Mart) on this ATM transaction data to understand the ATM usage pattern.


In this project , an ETL pipeline has to built using the following the steps

1)Extracting the transactional data from given MySQL RDS server to HDFS(EC2) instance using Sqoop.

2)Transforming the transactional data according to the given target schema using PySpark. 

3)This transformed data is to be loaded to  S3 buckets.

4)Creating the Redshift tables according to the given schema.

5)Loading the data from Amazon S3 to Redshift tables.

6)Performing the analysis queries.


**DATASET**

Source of the dataset in Kaggle : https://www.kaggle.com/datasets/sparnord/danish-atm-transactions


**Target Dimension model Schema**


<img width="610" alt="Screenshot 2024-02-23 230722" src="https://github.com/Smr-V/Spar-Nord-Bank-ETL-Pipeline/assets/47864256/bf8b3e18-9faa-4858-a070-b3ea383bf26b">







**ARCHITECTURE DIAGRAM OF THE ETL PIPELINE**





![Architecture Diagram](https://github.com/Smr-V/Spar-Nord-Bank-ETL-Pipeline/assets/47864256/9e0d1a0d-d17e-498a-bcb8-e1a42e68eb2e)
