# Call-center-Analysis 
A detailed analysis is conducted to give more transparency and insight into the data from the call centre . 
## Problem Description
To create a Power BI dashboard, that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset ,providing an accurate overview of long-term trends in customer and agent behaviour of the call centre.
## Project Goals
KPIs include:
•	Overall customer satisfaction.
•	Overall calls answered/abandoned
•	Total number of calls answered.
•	Total number of calls abandoned. 
•	Calls by time
•	Average speed of answer
•	Agent’s performance quadrant -> average handle time (talk duration) vs calls answered
•	Total number of calls resolved. 
•	Length of calls.

## Data Analysis Summary
Here is the dashboard i created,

![call centre dashboard PWC forage_page-0001](https://github.com/user-attachments/assets/65c6c841-9d0a-44e3-aaa9-3e43b4c3d2d4)
## Hardware and software used
• Mysql
• Windows 10 machine
• Microsoft Excel
• Microsoft PowerBI Desktop (v2.93)
## Explanation of Project Files
• 01 Call-Center-Dataset.xlsx - Original excel file containing call centre data.
• call centre dashboard.pbix - File contains the dashboard.

## Data 
The dataset includes  Call Id	,Agent,Date	,Time,	Topic,	Answered (Y/N),	Resolved,	Speed of answer in seconds,	AvgTalkDuration and	Satisfaction rating of different calls.
Time is set into 12 hour format with AM/PM. 
## Measure creation & Visualizations
• **Overall customer satisfaction** is found by averaging the satisfaction rating.
• **Calls answered and calls abandoned** are calculated from the Answered (Y/N) by
 ___Calls Answered = CALCULATE(COUNTROWS(Table1),Table1[Answered (Y/N)]="Y")___
 ___Calls Abandonded = CALCULATE(COUNTROWS(Table1),Table1[Answered (Y/N)]="N")___
 
• **calls by time**  : 
Measure named, **Total calls = count(Table1[Call ID])**
A new column named 'Time Interval' is created from the column 'Time' and plotted against Total calls on line plot.
• **Average speed of answer** is found out by averaging the speed of answer in seconds
• **Agents Performance Quadrant** is plotted by Talk duration vs calls answered on scatter plot.
• **Total number of calls resolved** 
___Calls resolved = CALCULATE(COUNTROWS(Table1),Table1[Resolved]="Y")___
• Average length of calls calculated by averaging the call durations.
The main visuals i used were slicers.i created date slicers as well as agent slicers to dive deep into the data.

## Conclusion
Using PowerBI I was able to visualize call centre data in an interactive way.



 
