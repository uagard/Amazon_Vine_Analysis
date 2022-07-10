# Amazon_Vine_Analysis

## Analysis Overview 

The purpose of this analysis was to use Pyspark to perform the ETL process to extract a video game reviews data set (DF written by memeber of the paid Amazon Vine program, a  service which allows manufacturers and publishers to recieve reviews for their products in exchange of a small fee), transform the data, connect to an AWS RDS instance, and finally load the transformed data into pgAdmin. In addition, PySpark was used to determine if there was any bias towards facorable reviews from vine member in the data set. All of this was done with the aim to undesrtand if the Amazon Vine program was worth the fees paid by manufacturers. 
 
## Software 
- PySpark 
- Google Collaboratory 
- Amazon Web Services (AWS)
- Postgresql 
- pgAdmin 
- Pandas 

## Results 

- How many Vine reviews and non-Vine reviews were there?
- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

The dataset had 1,785,997 reviews, however, only reviews with 20 or more votes were considered, norrowing the list to 65,379 , in addition helpful votes were defined as being 50% or greater than the total votes, which narrowed the list to 40,565.

![paid_vine_votes](https://user-images.githubusercontent.com/98793962/174197413-737d0867-effb-42d7-937c-ed01ea67a5b8.png)

![unpaid_vine_votes](https://user-images.githubusercontent.com/98793962/174199879-be74d31a-70bd-4af3-821c-8e555288d12e.png)

Regarding paid vine reviews, only 94 revies were filtered out as paid, 48 of those being 5 star reviews. This accounts for a 51.06% of 5-star paid vine program reviews.

Regarding the unpaid vine reviews, 40,471 reviews were filtered out as unpaid, 15,663 of those were 5 star reviews, accounting to a 38.7% of 5-star reviews. 

## Summary 
There is a grand difference in the number of reviews between both paid and unpaod reviews. The difference is too big, thus making it biased towards paid reviews, however, paid reviews has a higher percentage of 5 star reviews than the unpaid vine program. 
