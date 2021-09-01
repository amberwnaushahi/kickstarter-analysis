**Kickstarting with Excel**

*Overview of Project*

The purpose of this exercise was to analyze data from over 4,000 crowdfunding projects to help Louise understand how different campaigns fared in relation to their launch dates and funding goals. For the comparison of launch dates, the analysis was undertaken on the parent category “theater” and for funding goals, it was based on the subcategory “plays”. The outcomes of campaigns included “successful”, “canceled” and “failed” and did not include “live” for the analysis. 

*Analysis and Challenges*

*Analysis of Outcomes Based on Launch Date*

To perform the analysis of outcomes based on launch date and be able to visualize the campaign outcomes (“successful”, “failed” and cancelled”), I:

1-	Extracted the year from the “Date Created Conversion” column using the YEAR(). This helped me present the outcomes by month.

2-	Created a pivot table from the Kickstarter worksheet to condense the data and present a summary of outcomes based on launch date. 
Note: Relationships across time-related fields are automatically detected and grouped together when you add rows of time fields to your PivotTables. To show the months of the year, row labels can be grouped.  
 
3-	The fields that are chosen determine how the information is displayed in the pivot table. Since I wanted to see how the theater category fared, I applied the filter to the parent category and sorted campaign outcomes in descending order.
 
4-	To add visualization to this data and understand the relationship between outcomes and launch month, I created a line chart:

![image](https://user-images.githubusercontent.com/87351928/131610058-c48781ca-64e7-457d-94de-a0f8f110f660.png)
 
*Analysis of Outcomes Based on Goals*

To perform the analysis of outcomes based on campaign goals and be able to visualize the campaign outcomes (“successful”, “failed” and cancelled”) in the “plays” sub-category:

1-	I first created a new worksheet called “Outcomes Based on Goals” and populate it.

2-	Defined column headers as:
o	Goal
o	Number Successful
o	Number Failed
o	Number Canceled
o	Total Projects
o	Percentage Successful
o	Percentage Failed
o	Percentage Canceled

and defined the goal ranges in order to group projects based on their goal amount.

3-	We then populate the table, by using a COUNTIFS() function on “Number Successful”, “Number Failed” and “Number Canceled”. A COUNTIFS() function helps count the number of items from a dataset that meet multiple criteria. In this case, we use the function to count the number of crowdfunded projects in the “plays” sub-category that were successful, canceled or failed under each goal range. 

I also used the SUM() function to find the total number of projects in each goal range, and calculate the respective percentages in column F, G and H.

4-	To add visualization to this data and understand the relationship between outcomes and goals, I created a line chart:

![image](https://user-images.githubusercontent.com/87351928/131610083-69a2cc39-f5c1-4b4b-9838-8edd2d435615.png)
 
*Challenges and Difficulties Encountered*

While no challenges were encountered during the analysis, there are several issues that could arise:

1-	Incorrect fields applied to the rows and columns in the pivot table fields. This will present the pivot table differently and the most appropriate analysis, as warranted by the situation, may not be apparent or relationship may not be established based on the parameters defined. 

2-	As mentioned before, relationships across time-related fields are automatically detected and grouped together when you add rows of time fields to your PivotTables. This can present a challenge and lot of trial and error may be required to get to the relevant data field, months in this case. 

3-	The line charts may not be picked up correctly if the cell formatting is incorrect or incorrect range is chosen. 

4-	The data in the pivot table may not be presented correctly and the design tab will need to be used to ensure the correct headers etc are applied.

*Results*

Outcomes based on Launch Date

o	Based on the line graph, it seems that the key months to launch a successful theater project are May and June, accounting for 25.1% of total successful campaigns. This serves as an ideal time to launch a campaign. 

o	The successful outcome continues to decline for the rest of the year, after June. The high failure outcome towards the end of the year could be attributed to limited family budgets as a result of holiday spending. It is not the best time to launch a campaign. 

Outcomes based on Goals

o	It would appear that the highest percentage of successful outcomes in the “plays” sub-category has been for projects with either a goal of less that $5,000 (73.4% success rate) or between 35,000 and $50,000 (66.7%). 

o	A campaign has better chances to succeed in getting funded with lower budgets. Almost 90% of the plays that were successfully funded had a goal of less than $10,000. 

*Limitations of this dataset*

o	One limitation of this dataset is the date format for the date created and date ended. These had to be converted to a date format, that was understood by anyone looking at it.

o	There is limited information on how these fundraising campaigns were performed i.e. online donations, in-person or phone. It may be useful to see what medium had the highest success rate which could help Louise devise her fundraising strategy more effectively. 

*Recommendation for additional tables or graphs*

Additional graphs and tables could help identify additional factors that contribute to the success of a campaign. 

o	Data could be analyzed for other sub-categories within the theater parent category to determine trends or even for other parent categories. This could help determine if Kickstart is actually a useful platform for raising money  

o	A pivot table and line graph to analyze relationship between staff picks (which seem to enjoy more success) and campaign outcome 

o	In both analyses, the spotlight and staff pick were not investigated for impact on outcomes. 

o	Looking at outcomes based on duration of campaign could also help Louise determine her fundraising strategy. 
