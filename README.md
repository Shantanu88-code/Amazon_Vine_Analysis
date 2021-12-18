# Amazon_Vine_Analysis

# Analysis Overview:
We are analysing a larger project, analysing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. We also use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in dataset. For our analysis, we are performing ETL on sports products dataset.

# Results

We first filter our dataset with total votes equal to or greater than 20

<img width="423" alt="review20" src="https://user-images.githubusercontent.com/86980240/146649868-4bffe932-080b-4211-899c-1f35d801b531.png">

After we transform filtered data further we find following outcomes.

# How many Vine reviews and non-Vine reviews were there?

<img width="869" alt="vine_nonvine" src="https://user-images.githubusercontent.com/86980240/146649956-0b2a3066-2166-4592-afd5-0c9fdb555c6b.png">

There were a total of 61,948 reviews on sports products. Out of those, only 334 were vine reviews and 61,614 were non vine reviews. The total number of five star reviews were 32,804.

# How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

As mentioned above there were 32,804 five star reviews out of which, 139 were vine reviews and a significant 32,665 were non-vine.

<img width="872" alt="five-paid-unpaid" src="https://user-images.githubusercontent.com/86980240/146650152-3c9bd38d-cee1-42d0-8898-f28d08561ee7.png">

# What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

<img width="874" alt="percent" src="https://user-images.githubusercontent.com/86980240/146650186-669bc543-b075-45ed-ad26-eb5afa7db600.png">

There were 0.42% vine reviews and 99.58% non-vine reviews.

