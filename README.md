# Amazon Vine Analysis
## Overview
We choose a dataset that contained reviews of a specific project, I chose to look at reviews of cameras. We then performed the Extract, Transform, Load process to transform the data, connecting to an Amazon Wed Services Relational Database, and loaded the transformed data into pdAdmin. We used PySpark to look for any bias towards favorable reviews from Vine members.
## Resources
- Data: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Camera_v1_00.tsv.gz
- Tools: AWS RDS instance; pgAdmin; Google Colab; PySpark
## Results
The process of looking analyzing reviews for bias resulted the following:
- Total Vine Reviews: 607
- Total Non-Vine Reviews: 50522
- 5-Star Vine Reviews:257
- 5-Star Non-Vine Reviews: 25220
- Percentage of Vine Reviews that were 5-Star: 42.34%
- Percentage of Non-Vine Reviews that were 5-Star: 49.92%
## Summary
The first thing that stands out is the massive difference between the number of Vine Reviews compared to Non-Vine Reviews. It does seem that the sample size is still large enough to view on a large scale. We did see a larger percent of reviews as 5 stars in the Non-Vine users. While there is a difference, it's close enough in my opinion that further analysis needs to be performed to determine the significance of this difference. There are still plenty of places we can look at this data to form a more comprehensive analysis of our data set, such as looking at the percentage of reviews for each star level, the average star of each user group, and the summary statistics for each group.
