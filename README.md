# Amazon_Vine_Analysis
## Analysis Overview
The purpose of this project is to use Pyspark to perform the ETL process on Amazon reviews written by
members of the Amazon Vine program. Once the data is extracted and transformed, an AWS RDS instance was
connected so the transformed data could be transferred into pgAdmin. Lastly, Pyspark was used again to 
determine if there is any bias toward favorable reviews from Vine members in the dataset. The link to
the dataset is provided below. <br> 

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz

## Results
Based on the DataFrames that were generated from the dataset, there were several questions that needed
to be answered.

- How many Vine reviews and non-Vine reviews were there?

<h3 align="center">Vine Reviews</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/Vine_reviews.png"/>
</p><br>

<h3 align="center">Vine Count</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/Vine_count.png"/>
</p><br>

The images for the Vine member reviews DataFrame and the count are displayed above showing a count of 94.

<h3 align="center">non-Vine Reviews</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/non-Vine_reviews.png"/>
</p><br>

<h3 align="center">non-Vine Count</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/non-Vine_count.png"/>
</p><br>

The images for the non-Vine member reviews DataFrame and the count are displayed above showing a count of 40471.


- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

<h3 align="center">Vine 5-star Reviews</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/Vine_five_star_reviews.png"/>
</p><br>

<h3 align="center">non-Vine 5-star Reviews</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/non-Vine_five_star_reviews.png"/>
</p><br>

As seen in the images above, there were 48 5-star reviews by Vine members and 15663 non-Vine member reviews. 


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

<h3 align="center">Percent Vine 5-star Reviews</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/Percent_Vine_five_star_reviews.png"/>
</p><br>

<h3 align="center">Percent non-Vine 5-star Reviews</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Amazon_Vine_Analysis/blob/main/Resources/Percent_non-Vine_five_star_reviews.png"/>
</p><br>

As seen in the images above, about 51.1% of Vine member reviews were 5-stars and about 38.7% of non-Vine member 
reviews were 5-stars.

## Summary
