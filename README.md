# Kickstarter-analysis
Analysis of Kickstarter dataset 
## Overview of Project
Using the Kickstarter dataset, the Theater Outcomes Based on Launch Data was analyzed in excel to determine trends in the success, failure or cancelation of projects based on the launch date. Additionally, The Outcomes Based on Goals was analyzed in excel to determine trends in the success, failure or cancelation of projects based on project goals.

### Purpose

The purpose of this report is to determine project success of failure in relations to project launch date and their funding goals. The report will summarize outcomes based on project launch in a table and line graph. Additionally, the report will summarize outcomes based on funding goals in a table and line graph. 

## Analysis and Challenges

Prior to the analysis of Kickstarter dataset, the worksheet was cleaned and edited. The “Category and Subcategory” was broken into two new variables called “Parent Category” “Sub Category”. The “Deadline” and “Launched_at” variables were converted from a Unix timestamps into a data-month-year format. The new variables were named “Date Created Conversion” and “Date Ended Conversion”. A new variable was created for launch year by using the Year() function in excel, the new variable was called “Year”

### Analysis of Outcomes Based on Launch Date

A Pivot table was created in excel using “Parent Category” and “Years” as filters; “Date Created Conversion” as rows; and “Outcomes” as columns. The vales of the table are the “Count of Outcomes”. The Parent Category of the table was filtered to only display projects that fell into the theater category. The Pivot table breaks down the number of successful, failed and canceled projects by month. A line Chart named “Theater Outcomes Based on Launch” [Theater_Outcomes_vs_Launch.png](https://github.com/AjaniBenoit/Kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)Date was created to visualize data. The data revealed that most successful theater projects were launched in May with a total of 111 successful projects, 52 failed projects and 3 canceled projects. December was the least successful month to launch a theater project with a total of 37 successful projects, 35 failed projects and 3 canceled projects 

### Analysis of Outcomes Based on Goals

A new worksheet was created in excel called “Outcomes Based on Goals. A dollar-amount range was created to group projects based on their goal amount. The COUNTIFS() function was to populate the number of successful, number of failed and number of canceled projects based on the dollar amount range that fell into the subcategory of Plays. The SUM() function was used to calculate the total number of successful, failed and canceled projects. The percentage of the number of successful, failed and canceled projects was calculated. The line chart “Outcomes Based on Goal” [Outcomes_vs_Goals.png](https://github.com/AjaniBenoit/Kickstarter-analysis/blob/main/Outcomes_vs_Goals.png) shows the percentage of projects that were successful and the percentage of projects that failed at each dollar-amount range. The charts shows that projects with lower goals were more successful than projects with higher goals. 

### Challenges and Difficulties Encountered

No difficulties were encountered during the analysis of the data set. However possible difficulties can be encountered, for example failing to convert the Unix timestamp into a data-month-day-year format would prevent the analysis of the project outcomes based on the project launch date. Additionally, typos in the functions may result in incorrect values. To prevent human error, it is important to verify commands. 

## Results

###  Conclusion

 -	More projects were launched in May with a grand total of 166 projects. December saw the lowest number of projects launched with a total of 75 projects. 
-	Most successful projects were launched in May with a total 111 successful projects, 52 failed projects and 3 canceled projects. Conversely, December was the least successful month to launch a theater project with a total of 37 successful projects, 35 failed projects and 3 canceled projects. 
-	Plays with lower goals were more likely to have successful outcomes than plays with higher goals 
-	There are some limitations regarding the dataset. The Outcomes Based on Goals line chart displays the total successful and failed projects as percentage at each dollar amount range. Between the ranges 35000 to 39999 and 40000 to 44999 the percent of successful projects is 67 percent. A closer look of the data reveals that total of number of projects at those ranges was 6 and 3 respectively with the number of successful outcomes being 4 and 2 respectively. Presenting this as a percentage skews the data. Future analysis of data on Outcomes Based on Goal should include therefore include a Box and Whiskers Plot to help identify the median goal and outliers. 

