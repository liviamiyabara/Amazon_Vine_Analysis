# Amazon_Vine_Analysis
Module 16: Big Data

## Overview of the analysis

In this week's challenge, the student analyzes Amazon reviews. There is a program called Amazon Vine, where sellers pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. 

In the first section of the challenge, the student selected the Amazon review database for Furniture, the data is extracted from S3, transformed through Pyspark and then loaded to PG Admin. [Link to ETL code.](https://github.com/liviamiyabara/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)

The second portion of this week's deliverable is to develop an analysis to understand if there is any bias toward favorable reviews from Vine (paid) members. [Link to Vine Review Analysis.](https://github.com/liviamiyabara/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)

## Results

* How many Vine reviews and non-Vine reviews were there?
    
    There are 136 Vine reviews in the furniture dataset and 18,019 reviews from non-Vine members
    
* How many Vine reviews were 5-stars? How many non-Vine reviews were 5-stars?
    
    There were 74 5-star reviews from Vine members and 8,482 5-star reviews from non-Vine members

* What percentage of Vine reviews were 5-stars? What percentage of non-Vine reviews were 5 stars?
    
    The percentage of Vine reviews for 5-stars was 54%

    The percentage of non-Vine reviews for 5-stars was 47%

Details on calculation can be found below:
![ScreenShot](https://github.com/liviamiyabara/Amazon_Vine_Analysis/blob/main/Resources/calculations.JPG)

## Summary

The percentage of 5-star reviews from the paid Vine members was 54% and for the non paid reviewers it was 47%. Although the higher percentange from the paid members could indicate a possible bias of posivite reviews, addtional statistics analysis is recommended. An ANOVA test could be executed to understand if the difference between the 2 groups (Vine members and non-Vine members) have a statistical difference between the number of 5-star reviews. 
