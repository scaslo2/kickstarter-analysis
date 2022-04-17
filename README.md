#Excel Analysis on Kickstarter Campaigns

##Overview of Project

For this project I analyzed the given data set on kickstarter campaigns, starting from 2009 until 2017. I was given data on how much a campaign's goal was, how much was actually pledged, the outcome of the campaign - was it successful or not - as well as the category of the proposed campaign - was it for a television show, theater show, drama, etc. For this analysis, I chose to focus on theater kickstarter campaigns.

###Purpose

The purpose of my analysis was to look at historical data on theater kickstarter campaigns. I wanted to see how successful or not a campaign was based on when the launch date was as well as how much the projected goal amount was. 


##Analysis and Challenges
###Analysis of Outcomes Based on Launch Date

I had to first use the "=year()" function in Excel to extract the year from the start date column in the data set. From here I chose to create a pivot table, using the "Parent Category" - then choosing the theater category - and "Years'' columns as filters. Afterwards, I chose "Outcome" for the column and "Start Date" as the row. I had to manipulate the rows to show by month. This separates the data, giving the total number of successful, failed, and canceled theater shows from 2009-2017, by month. Being that the data is linear, I chose a line chart to best showcase the outcomes.

###Analysis of Outcomes Based on Goals

In order to effectively analyze outcomes based on goals, I had to create 12 unique ranges, from <$1000 to >$50,000, with $5,000 intervals. From here, I used the "=countifs()" function to count the number of successful, failed, and canceled theater shows by the quantity of the goal. For example, I counted the number of successful theater shows whose goals were between $5,000 and $9,999 and got a total of 93. 

I then used the "=sum()" function to find the total number of projects within each goal range and with this I was able to find the percentage of successful, failed, and canceled theater shows as well. I used my findings to create a line chart that showcased the percentage of successful, failed, and canceled theater shows by goal range. 


###Challenges and Difficulties Encountered

I experienced two challenges during my analysis. The first was finding out how to break down the outcomes based on the launch date pivot table to show only the months instead of year and month. I had to first enter the start date column within the values section of the pivot table and then take away years. The other major issue I had was finding the best way to break down the goal ranges within excel that would allow me to write my function in a way where I could drag it down across multiple rows and it would adjust appropriately, allowing for a quicker analysis. To best do this, I chose to use the surrounding cells to hold certain key data points and write out my function to use these cells as absolute references. 


##Results
###What are two conclusions you can draw about the Outcomes based on Launch Date?

The first conclusion I can draw from the outcomes based on launch date is that the summer is the best time to launch a theater show. You can tell by the number of successful shows in June, July and August - all three months having more than 90 successful shows. The other conclusion I came to was that very few shows get canceled - in fact in April, zero shows were canceled. 

###What can you conclude about the Outcomes based on Goals?

After analyzing the outcomes based on goals data, I can conclude that shows with a goal less than $15,000 and goals between $35,000 - $50,000 tend to have a high success rate, while goals between $20,000 and $35,000 and any goals greater than $50,000 have a much higher failure rate. However the cancellation rate across all ranges is negligible. 

###What are some limitations of this dataset?

Given that we are only looking at about 1,000 theater shows over 18 years, it is hard to have a high confidence level in this data. Given the amount of time, you would expect to have more theater shows in the dataset.

###What are some other possible tables and/or graphs that we could create?

A box and whisker chart would work well in showing the mean, median and distribution of successful vs failed theater shows by goal quantities. 


