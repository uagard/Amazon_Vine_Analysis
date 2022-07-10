# Amazon_Vine_Analysis

## Analysis Overview 

The objective for this analysis was to use Pyspark to perform the ETL process to extract a video game reviews data set. The dataframe was written by memebers of the paid Amazon Vine program. This is a service that will allow the manufacturers and publishers to receive reviews for their products in exchange of a small fee. We are to  transform the data, connect to an AWS RDS instance, and finally load the transformed data into pgAdmin. PySpark is used to determine if there was any bias towards favorable reviews from the vine member in the data set. All of this was done with the aim to understand if the Amazon Vine program is the worth the fees paid by the manufacturers. 
 
## Software 
- PySpark 
- Google Collaboratory 
- Amazon Web Services (AWS)

## Results 

- How many Vine reviews and non-Vine reviews were there?
- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Overall the dataset has 1,785,997 reviews. For the sake of the project, only reviews with 20 or more votes were considered. Once the was done it narrowed the list to 65,379 reviews. In addition helpful votes were defined as being 50% or greater than the total votes, which narrowed the list to 40,565.

Regarding paid vine reviews, only 94 revies were filtered out as paid, 48 of those being 5 star reviews. This accounts for a 51.06% of 5-star paid vine program reviews.

Regarding the unpaid vine reviews, 40,471 reviews were filtered out as unpaid, 15,663 of those were 5 star reviews, accounting to a 38.7% of 5-star reviews. 

## Summary 
There was a large difference in the number of reviews between both paid and unpaod reviews. The difference shows that there was a bias towards paid reviews, but, paid reviews has a higher percentage of 5 star reviews than the unpaid vine program. 
