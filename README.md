# Amazon_Vine_Analysis

## Overview of the Analysis

In this analysis, we are working with Amazon Vine reviews. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their projects. 

We were given access to about 50 datasets each, wherein, each dataset contains reviews for a specific category. Using PySpark and the Postgres, we created a database that underwent the ETL process in order to clean and query data that will be of use to Amazon Vendors.

This analysis focuses on the Video Game dataset.

## Results

![Amazon Vine Summary Stats](https://github.com/patrickryanpo/Amazon_Vine_Analysis/blob/main/Resources/Results%20Summary.png)

As shown by the image, after going through the ETL process 40,565 reviews were left remaining. We wanted to see the number of 5-star reviews in the qualified dataset, which came out at 15,711 reviews. With this information, we segregated Vine users from Non-Vine users. Total 5-Stars from vine users was found to be at 48, on the otherhand, 5-star non-vine users resulted in 15,663. Given this data, we can say that majority of the video game reviewers on Amazon are non-Vine reviewers. The data is more precisely illustrated by the percentages. 0.31% of video game reviewers who gave 5-Stars are vine reviewers, and 99.69% are non-vine users. 

## Summary 

Based on the findings, there were barely 5-star any vine reviewes for the video game category. We could say that there is a heavy bias towards non-vine reviewers. In order to improve the accuracy of the reviews, it would be important to balance this figure out. 

For the category of video games, I would suggest to perform analysis on the verified purchase column. Segregating reviewers who have actually purchased and not purchased might bare more fruitful results. In addition to this, we can also look at the trend for lower star ratings for both vine users and non-vine users. By doing this and comparing the results to our positive bias, we will be able to gain a deeper understanding of the relevance of our vine reviews for the category. 

### Postgres Tables

Below are screen shots of the data samples available in our Postgres database. 

![Customers Table](https://github.com/patrickryanpo/Amazon_Vine_Analysis/blob/main/Resources/Customers%20Table.png)
![Products Table](https://github.com/patrickryanpo/Amazon_Vine_Analysis/blob/main/Resources/Products%20Table.png)
![Review ID Table](https://github.com/patrickryanpo/Amazon_Vine_Analysis/blob/main/Resources/Review%20ID%20Table.png)
![Vine Table](https://github.com/patrickryanpo/Amazon_Vine_Analysis/blob/main/Resources/Vine%20Table.png)

