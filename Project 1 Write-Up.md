# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this project is to analyze different Kickstarter campaigns in order to identify trends in launch dates and frundraising goals in the context of their relation to campaign outcomes.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To create my analysis of outcomes based on launch dates, I created a pivot table using the Kickstarter data, filtering by parent category and years, using the campaign start dates as rows, and the outcomes (successful, failed, or canceled) as columns. Based off the pivot table, I then created a line graph with the campaign start date on the x-axis and the count of outcome on the y-axis.

### Analysis of Outcomes Based on Goals
To create my analysis based on goals, I created countifs formulas to count the number of campaigns based on outcome that fell within a certain goal range. Once I set up my formulas for column B, I dragged the formulas to the right, populating columns C and D. I used the Find and Replace feature to replace the "successful" criteria with "failed" and "canceled" criteria, respective to their corresponding columns. To find the total number of projects, I used a sum formula to capture data to the left. I calculated the percentages by dividing the number based on category & goal by the corresponding "Total Projects" value. From my newly populated data, I created a line graph with the goal ranges on the x-axis and the percentages on the y-axis.

### Challenges and Difficulties Encountered
I initially ran into issues using the Countifs formula because I didn't remember how the formula was supposed to be set up. Originally I was trying to use the formula Countifs(Kickstarter!$F:$F="successful",Kickstarter!$D:$D<1000). By watching the countifs formula video, I was quickly able to realize how I had set up the formula wrong and corrected it.

Another small issue I can into was how to set up the formula for the "greater than 50,000" category. Just based off of the name "greater than 50,000" I would think that the value would have to be greater than 50,000 and not equal to exactly 50,000. However, if I set up the formula to be strictly greater than 50,000, then no category would capture the 50,000 data point (the previous category is 45,000 to 49,999). Because of this, I made sure the formula captured the 50,000 data point as well.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Based on the launch date analysis, it is clear that campaigns in the May to July months are the most successful , while failed campaigns hover around 40% funding year-round. While there isn't much correlation between the campaign start month and failed campaigns, there definitely is a clear trend when looking at successful campaigns. While launch date may not have any effect on a campaign that's destined to fail, it can definitely help determine just how successful a successful campaign will be. 

- What can you conclude about the Outcomes based on Goals?
As the fundraising goal increases, so does the percenatge of failed campaigns. The higher the goal, the more likely the campaign is to fail. 

- What are some limitations of this dataset?
The data is a bit old (ends in 2017) and could be not as relevant in regards to fundraising today and the much different climate we live in. For instance, a live play fundraising campaign today would likely have a hard time being successful due to covid and obstacles that social distancing creates.

The most glaring limitation of the dataset is how success is defined. I could hypothetically create a bunch of fundraising campaigns with goals of $5 and they would all be successful because of how low and achievable the goal is. Because the goal amount can be so abritrary in some senses, and due to the fact that all of the analyses are based off the goal amount and associated campaign sucess, the overall analyses could be very flawed. 

- What are some other possible tables and/or graphs that we could create?
We could look at the effect of staff picks, as well as the effect of campaign spotlights, on campaign outcomes. The relationships could be displayed on two seperate bar graphs. 
