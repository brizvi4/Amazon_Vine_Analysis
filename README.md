# Amazon Vine Analysis

## Overview

In this module, I analyzed Amazon reviews written by members of the paid Amazon Vine program. My job was to determine if there were any biases between Vine members and non-Vine members' reviews. Companies would pay a fee to Amazon and may provide free products to Vine members who are then required to publish a review. In order to determine if there is any bias towards favorable reviews from Vine members, I chose a dataset from a list of 50 Amazon datasets and extracted, transformed and loaded this dataset into a dataframe in order to complete my analysis. For this module, I applied my skills in the following tools: PySpark, AWS RDS, pgAdmin, SQL and PostgreSQL.

## Results

For my analysis, I first filtered the total votes count to greater than or equal to 20 votes in order to pick reviews that are more likely to be helpful.

<img width="386" alt="Pic1" src="https://user-images.githubusercontent.com/95254809/170417910-33cc643d-2491-4975-ae03-6a9be120fb2d.PNG">

Then I further filtered the above dataframe to retrieve all the rows where the number of helpful_votes divided by total_votes was equal to or greater than 50%.

<img width="601" alt="Pic2" src="https://user-images.githubusercontent.com/95254809/170418728-c338e724-6fbd-4af1-b0af-b378501d5372.PNG">

Finally, I found out total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for both Vine program members and non-members. Following were the results:

<img width="406" alt="Pic3" src="https://user-images.githubusercontent.com/95254809/170418831-595e019a-2e95-4dcf-93d1-d3a48fdb08f8.PNG">

## Summary

Based on the results of the final table, there does seem to be a bias since paid members had 41.13% of 5 star reviews whereas non-paid members had 29.4% of 5 star reviews. At the same time, more datasets should be analyzed. I did a lot of filtering in this dataset, so I would not definitely conclude by saying that there was a bias when it comes to paying people in the Vine program. 




