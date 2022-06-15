# Amazon Review Analysis 

## Amazon Review Analysis Overview
#### As a massive retail company, Amazon relies on customer reviews to maintain ongoing sales. One way Amazon ensures the products are reviewed is through their Amazon Vine program, which pays select consumers to trial a product and then post a review of the product. However, as these reviews are sponsored by Amazon, Amazon is looking to evaluate if this affects the reviews provided by Vine members. To do this, information about furniture items was extracted through PySpark, transformed utilizing Pandas, and then loaded into a csv via PostgreSQL for further analysis. From there, five-star reviews were evaluated for both Vine (paid) reviews, and unpaid reviews.

## Resources Utilized
##### Data Source: [Amazon Furniture Review Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Furniture_v1_00.tsv.gz)


##### Software: Python 3.7.6; Anaconda 4.10.3; PgAdmin 4; PostgreSQL 11, PySPark 3.0.3, AWS and RD3


## Amazon Review Results
#### Based on the furniture review data analyzed, several results can be noted for Vine (paid) reviews and unpaid reviews. The image below references the calculations utilized to answer the following questions.

![Vine_Review](https://user-images.githubusercontent.com/99554642/173878652-4881e299-eb22-4a26-96e6-b30b3523e08e.png)




* How many Vine reviews and non-Vine reviews were there?


*In the furniture review dataset, there were 157 total Vine reviews and 24,709 total unpaid reviews.*

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?


*There were 84 5-star Vine reviews and 11,930 5 star unpaid reviews.*

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?


*Overall, 53.5% Vine reviews were 5-star reviews and 48.3% of unpaid reviews were 5 star reviews.*


## Amazon Review Analysis Summary
Based on the furniture review dataset, there does appear to be positivity bias in the reviews provided by the Vine program members. Out of all the Vine reviews, 53.5% were 5 stars, whereas the unpaid reviews exhibited only 48.3% of reviews consisting of 5-star reviews. The paid reviews show a higher rate of 5-star reviews, however that could be only true for this dataset, as furniture products may yield different responses then other products sold by Amazon. 
Another analysis could be run to determine the percentage of other reviews provided by Vine and unpaid reviews. Perhaps Vine reviews have a higher percentage of 0 or 1-star reviews and unpaid reviews have a higher percentage or 3 or 4-star reviews. Conducting analysis on the percentages of other ratings could provide better insight on the level of positivity bias demonstrated by Amazon’s Vine program.
