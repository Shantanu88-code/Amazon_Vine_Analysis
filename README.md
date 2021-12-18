# Amazon_Vine_Analysis

# Analysis Overview:
We are analysing a larger project, analysing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. We also use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in dataset. For our analysis, we are performing ETL on sports products dataset.

# Results

We first filter our dataset with total votes equal to or greater than 20

<img width="524" alt="review20" src="https://user-images.githubusercontent.com/86980240/146652453-8beeabb7-df31-415d-bec8-8793589bbac5.png">

After we transform filtered data further we find following outcomes.

# How many Vine reviews and non-Vine reviews were there?

<img width="615" alt="total1st" src="https://user-images.githubusercontent.com/86980240/146652411-3b12c700-c53e-4829-afbe-7dde7553a0f8.png">
<img width="562" alt="vine_nonvine" src="https://user-images.githubusercontent.com/86980240/146652430-f126a42a-57ca-4eb7-9c24-ab2b0af71af7.png">

There were a total of 61,948 reviews on sports products. Out of those, only 334 were vine reviews and 61,614 were non vine reviews. The total number of five star reviews were 31,939.

# How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

As mentioned above there were 32,804 five star reviews out of which, 133 were vine reviews and a significant 31,806 were non-vine.

<img width="666" alt="five-paid-unpaid" src="https://user-images.githubusercontent.com/86980240/146652463-cbaf547c-ceca-4793-9499-4f53d034ae0a.png">

# What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

<img width="659" alt="PCT" src="https://user-images.githubusercontent.com/86980240/146652485-23eac740-9a0e-4faf-8f94-72894ed0af6a.png">

There were 39.82% vine reviews and 51.62% non-vine reviews.

