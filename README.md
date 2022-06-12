# Amazon Product Reviews

## Analysis of the reviews from Amazon's Vine program

### Overview of the Project

The purpose of this project is to analyze the Amazon reviews written by members of the paid Amazon Vine program.  This program allows manufactures and publishers to receive reviews for their products.  Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are required to publish a review.

This analysis will review the data to determine if there is a bias of the program members to provide a favorable review vs. reviews received from program non-members.

For this project I chose to analyze reviews that were made by users in the "Kitchen" category.  

### Results:

The dataset had 4,880,466 million reviews collected.  The data was cleaned using the dropna function to filter out null values, this reduced the dataset to 4,879,961.  The data was also cleaned using the .drop_duplicates() function to ensure reviews were only counted once.  However, there were no duplicates so the dataset remained at 4,879,961.

![Cleaned Dataset](https://user-images.githubusercontent.com/99366022/173215933-7ea3baec-4776-4c6a-9f4e-d3b52121e72c.png)

The data was filtered in order to focus the analysis on reviews that would help provide answers of the analysis.  For the analysis reviews with a count of "Total_Votes" equal to or greater than 20 were included.

![20 Total Votes](https://user-images.githubusercontent.com/99366022/173216900-9081e5c5-1d5f-4e86-8229-3bb4e3ac3d72.png)

We also looked at the number of "helpful_votes" and included the reviews where the number of helpful votes were equal to or greater than the total_votes.

![50 percent helpful votes](https://user-images.githubusercontent.com/99366022/173216972-95788701-8a2c-4fdf-bb2e-b2619d451ee1.png)

There were 99,017 reviews included in the final analysis.  Answers to the following questions were discovered as part of the review:

1. How many Vine reviews and non-Vine reviews were there?
- There were 1,207 (1.2%) vine member reviews

![VineProgramMember](https://user-images.githubusercontent.com/99366022/173217621-8a501d97-27bf-4569-8778-69c49ae1d871.png)

- There were 97,810 (98.8%) vine non-member reviews

![VineProgramNonMember](https://user-images.githubusercontent.com/99366022/173217674-3776e957-26ab-4abf-b4d5-f752d5f855ed.png)

2. How many Vine reviews received 5-stars?  How many non-Vine reviews received 5-stars?
- Of the 1,207 member reviews 509 received a 5-star rating
- Of the 97,810 non-member reviews 45,810 received a 5-star rating

3. What percentage of the Vine reviews received 5-stars?  What percentage of non-Vine reviews received 5-stars?
- 42.2% of the member reviews received a 5-star rating
- 46.9% of the non-member reviews received a 5-star rating

![Total_Reviews](https://user-images.githubusercontent.com/99366022/173217327-70b31d36-fc20-4857-88e1-031a528f0f21.png)

### Summary
Based on the results of the analysis Vine program members did not show a bias for giving 5-star ratings.  The significant number of non-member reviews included in the analysis and the higher percentage of 5-star ratings support the statement of no bias.

This statement could further be tested by conducting the same analysis on another set of data from the Amazon Vine program to see if the results shows the same results or not.

In the summary state if there is any positivity bias for reviews in the Vine program.  Use the results of the analysis to support the statement.  Then, provide one additional analysis that you could do with the dataset to suppport your statement.
