# BigData

### Overview of the analysis: Explain the purpose of this analysis.

The purpose of this analysis was to become familiar with Big Data. As part of this analysis, we were introduced to PySpark, Google Colabratory, AWS (both RDS and S3), and continued our work with PostgreSQL. We were asked to import data into Google Colabratory from our choice of the Amazon Review Datasets. From this choice of datasets, I chose the Apparel dataset. We were required to import the dataframes we created in Google Colabratory into an AWS Amazon Relational Database. In Google Colabratory, we were able to import the data from RDS into a SQL database in PostgreSQL. Next, we created dataframes to compare the paid and unpaid Vine reviews in the Amazon Review Dataset we chose. The final step was to determine if there is any positivity bias for the reviews in the Vine program. 

![Apparel Datafram](https://github.com/lllohr/BigData/blob/6671e23ff80b441eabbcb21cff37f670b4caff64/images/apparel_df.png)


![Customer Table in PostgreSQL](https://github.com/lllohr/BigData/blob/6671e23ff80b441eabbcb21cff37f670b4caff64/images/customers_table.png)


![Database View in PostgreSQL](https://github.com/lllohr/BigData/blob/6671e23ff80b441eabbcb21cff37f670b4caff64/images/database.png)


### Results: Using bulleted lists and images of DataFrames as support, address the following questions:

- How many Vine reviews and non-Vine reviews were there?

The apparel dataset I chose had a total of 5905269 reviews. Of the total number of reviews---46767 had a vote count of 20 or more, 45279 were considered helpful. There were 33 paid Vine reviews in that filtered set. There was 45246 unpaid Vine reviews in the filtered set. 

![Vine Table in SQL](https://github.com/lllohr/BigData/blob/6671e23ff80b441eabbcb21cff37f670b4caff64/images/vine_table.png)

![Vine Data Frame in Google Colabratory](https://github.com/lllohr/BigData/blob/6671e23ff80b441eabbcb21cff37f670b4caff64/images/vine_df.png)


- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

There was 15 paid Vine reviews with a 5 star review, while 23639 unpaid Vine reviews had a 5 star review.  

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

45.45454545454545% of paid Vine reviews had a 5 star rating, while 52.245502364849926% had a 5 star rating.

![Unpaid Vine Review](https://github.com/lllohr/BigData/blob/6671e23ff80b441eabbcb21cff37f670b4caff64/images/unpaid_vine.png)


### Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

I didn't see any positivity bias in the paid vs the unpaid review. 45% of Vine reviews that were paid had a 5 star rating and 52% of the unpaid had a 5 star rating. I think it would be beneficial to view the total reviews that were 3 stars or better for unpaid and paid reviews to see if that sheds some light on any potential bias. I also think the sample size was too low for the paid reviews to make any conclusive determinations of bias. Perhaps, we could look at the average of the reviews as well. 


