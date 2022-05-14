# Amazon_Vine_Analysis, Module 16 Challenge

Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.


## Deliverable 1: Perform ETL on Amazon Product Reviews 

The Amazon Review: **"Musical Instruments"** dataset was selected, and is extracted as a DataFrame.

![11](Images/11.png)

The extracted dataset is transformed into four DataFrames with the correct columns.

* Customer ID and Count

![12](Images/12.png)

* Product ID and Title

![13](Images/13.png)

* Review ID

![14](Images/14.png)

* Vine Table

![15](Images/15.png)

All four DataFrames are loaded into their respective tables in pgAdmin.

![160](Images/160.png)

![16](Images/16.png)

![17](Images/17.png)

![18](Images/18.png)

![19](Images/19.png)


## Deliverable 2: Determine Bias of Vine Reviews

There is a DataFrame or table for the vine_table data using one of three methods above.



The data is filtered to create a DataFrame or table where there are 20 or more total votes.



The data is filtered to create a DataFrame or table where the percentage of helpful_votes is equal to or greater than 50% (5 pt)



The data is filtered to create a DataFrame or table where there is a Vine review (5 pt)



The data is filtered to create a DataFrame or table where there isn’t a Vine review (5 pt)
The total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews (15 pt)




## Deliverable 3: A Written Report on the Analysis

Structure, Organization, and Formatting (6 points)

The written analysis has the following structure, organization, and formatting:
There is a title, and there are multiple sections (2 pt)
Each section has a heading and subheading (2 pt)
Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis (14 points)

The written analysis has the following:
Overview of the analysis of the Vine program:
The purpose of this analysis is well defined (3 pt)
Results:
There is a bulleted list that addresses the three questions for unpaid and paid program reviews (7 pt)
Summary:
The summary states whether or not there is bias, and the results support this statement (2 pt)
An additional analysis is recommended to support the statement (2 pt)