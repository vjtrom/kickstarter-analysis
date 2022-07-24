
![Category](https://github.com/vjtrom/kickstarter-analysis/blob/main/Category%2012-21.png)

![Date](https://github.com/vjtrom/kickstarter-analysis/blob/main/Date%20Created%207-21.png)

# Kickstarting with Excel

## Overview of Project
The overall goal of this project challenge is to assess the student’s competency in applying the skills and concepts presented in Module 1 – Kickstarting with Excel.

This is accomplished by using a case study where a young playwright, Louise, is seeking information and insights related to the crowdsource funding of her project - a play titled “Fever”. 

### Purpose

In this module challenge, the student will learn and apply excel skills and concepts that were covered in Module 1, including:
-	Evaluating data in excel
-	Creating pivot tables
-	Filtering and Formatting data
-	Understanding concepts and applying formulas related to Measures of Central Tendency, Measures of Spread, and Addressing outliers
-	Creating visualizations, including representing data in charts and tables

The student will attain a successful outcome by meeting the deliverables of this challenge, including the properly prepared and formatted spreadsheet, charts in .png format, and this written analysis.


## Analysis and Challenges

Using excel, the student was asked to utilize the data contained in the Kickstarter Challenge excel spreadsheet; analyze the data to identify patterns and trends; calculate and inspect data elements, including rates of campaign success and failure; evaluate categorical and time-series data; and provide insights and findings. 

### Analysis of Outcomes Based on Launch Date

In the analysis of Outcomes Based on Launch Date, the student was asked to prepare a summary of Subcategory “Theater” campaigns using the pivot table feature in excel. In order to make the launch date more useable, and in addition to converting Unix Timestamps into the Gregorian Calendar format month-day-year (MDY), the excel YEAR() function was use to further summarize the data. 

Once the data was summarized in the pivot table, the student was asked to create a chart of the Successful, Failed and Canceled projects by month, with the goal of determining which months produced the highest rates of success. 


### Analysis of Outcomes Based on Goals

In the Analysis of Outcomes Based on Goals, the student was asked to parse the number of Successful, Failed and Canceled projects by Goal, broken down into incremental ranges of $5,000. 

In order to achieve this, the student needed to use the COUNTIFS() function in excel, filtering on both categories and increments. In addition, the student needed to calculate the percentage of Successful, Failed and Canceled projects along these same increments. 


### Challenges and Difficulties Encountered

Since the data set was relatively large, with over 4,000 records, it was necessary to use filters and formatting in excel to aggregate and parse the data and make it more meaningful. Pivot tables were especially helpful in this area. In addition, some data strings had to be broken down using the Convert Text to Columns Wizard. This was essential in separating the ‘Categories’ data into ‘Parent’ and ‘Subcategory’, respectively. Another challenge was data cleansing, for example converting Unix Timestamps into readable formats. 


## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?

When looking at the ‘Theater’ category by launch date, it is clear that the months of May and June have the highest rates of success. Conversely, the rate of success for projects launched in November and December is lower. This is probably due to seasonality, with the impact of year-end holidays and possibly winter weather having a dampening effect on rates of success. The rate of Success peaks in May and June, and then steadily declines over the summer, with a slight uptick in October. All other things being equal, it is best to launch a campaign in late Spring. 

When looking at rates of failure, the results are spread out more evenly by month, which would suggest that some other factors other than month-of-year are involved in determining rates of failure. In addition, the ratio of successful to failed projects is roughly 2:1, and the number of canceled projects relative to Successful/Failed Campaigns is less than 3%.

### What can you conclude about the Outcomes based on Goals?

When looking at the Outcomes Based on Goals in the ‘Plays’ Subcategory, 96% of these have a project goal amount of $25,000 or less. In addition, only 4% of projects have a goal greater than $25,000. It is therefore easier to draw conclusions about plays with $25,000 or less due to the population size. 

Of the Plays with a project goal of $25,000 or less, the overall rate of success is 68%. For project goals of $10,000 or less, the rate of success is 70%, and for plays with project goals of less than $5,000, the rate of success is 74%.

This would suggest that all other things being equal, it is best to have a lower project goal in order to achieve a higher rate of funding success.

### What are some limitations of this dataset?

Some of the limitations of the data set include a wide dispersion of data by years (2009 – 2017), where conditions might change from year-to-year, such as economic conditions and public demand for theater projects. In addition, there are different countries with different currencies, which may not be seen as equivalent due to exchange rates and purchasing power. The length of projects, meaning the launch data compared to the deadline, may also be problematic, as certain projects may require a longer lead time, which in term may provide more time for a project to achieve its project goals. 


### What are some other possible tables and/or graphs that we could create?

Some other tables and graphs that might be useful include:
-  Breakdown by other categories
-	 Breakdown by Country
-	 % Funded by # of Backers filter
-	 % Funded by Category type
-  Best performing Subcategories within a Category
