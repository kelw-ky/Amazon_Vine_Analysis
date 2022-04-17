# Amazon_Vine_Analysis

## Overview 

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. We will be picking one out of 50 datasets and using PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we’ll use PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. The dataset, we choose, was Pets Products. 

## Datasets 

<b>Customers DataFrame & Customers Table</b>

<img src="/Resources/customers_df.png"/>
<img src="/Resources/customers_table.png"/>

<b>Products DataFrame & Products Table</b>

<img src="/Resources/products_df.png"/>
<img src="/Resources/products_table.png"/>
    
<b>Review ID DataFrame & Review ID Table</b>

<img src="/Resources/review_id_df.png"/>
<img src="/Resources/review_id_table.png"/>

<b>Vine DataFrame & Vine Table</b>

<img src="/Resources/vine_df.png"/>
<img src="/Resources/vine_table.png"/>

## Results

- <i>How many Vine reviews and non-Vine reviews were there?</i>
    - There are <b>170</b> Vine reviews. 
    ![Vine Reviews](/Resources/vine_reviews.png)

    - There are <b>37840</b> Non-Vine reviews. 
    ![NonVine Reviews](/Resources/nonvine_reviews.png)

- <i>How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?</i>
    - There are <b>65</b> 5 stars Vine reviews. 
    ![5s Vine Reviews](/Resources/vine_reviews_5s.png)

    - There are <b>20612</b> 5 stars Non-Vine reviews. 
    ![5s NonVine Reviews](/Resources/nonvine_reviews_5s.png) 

- <i>What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?</i>
    - <b>38.24%</b> are 5 stars Vine reviews
    ![Percent 5s Vine Reviews](/Resources/percent_vine_reviews.png)

    - <b>54.47%</b> are 5 stars Non-Vine reviews
    ![Percent 5s NonVine Reviews](/Resources/percent_nonvine_reviews.png) 

## Summary

It is clear that there are more 5 stars Non-Vine reviews than Vine reviews. This makes the reviews more reliable as the reviewers are not paid for this review allowing the reviews to be less influenced by the fact that they are being paid and will be more honest. 

In addition, we can test if the data is statistically significant of the star ratings of Vine and non-Vine reviews. This will show if the data is skewed or bias. 
