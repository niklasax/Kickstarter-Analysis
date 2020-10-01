# Kickstarting with Excel




## Overview of Project

### Purpose
The purpose of this project was to gain familiarity with Excel by sorting, analyzing, summarizing and visualizing data. In this particular example, we looked at kickstarter data with the ultimate goal of determining if there are certain factors, if any, that make a kickstarter funding campaign successful.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
For this analysis, we wanted to see if there was any correlation between the category's 'Theater' campaign's launch month and its success. We first took the raw data from the kickstarter tab and added a =YEAR() calculation at the end of the table to display only the year from the date created conversion. We also split 'category' and 'subcategory' into their own columns using the text to columns function. From there, we used the pivot function to filter and summarize our data. The pivot table was filtered to show only 'theater' from the parent category, 'date created conversion' was designated as the rows, 'outcome' was designated as the columns and count of outcomes was used for the values. Finally, we created a line chart from the pivot table with count of outcomes as the Y-axis, the months as the X-axis, and the different outcomes seperated by color.

### Analysis of Outcomes Based on Goals
For this analysis, we wanted to see if there was any correlation between the subcategory's 'plays' campaign's fundraising goal and its success. We first created a and a new column titled 'goal'. In the goal column, we created groupings of fundraising goals in increments of 5000, starting at 1000 or less and ending at 50000 or higher. Next, we created 3 calculated columns to determine the number of successful kickstarters, the number of failed kickstarters and the number of canceled kickstarters from the 'plays' subcategory. To do this, we used the =COUNTIFS function to count occurences from the kickstarter table if they met certain criteria based on 'goal' column groupings and whether it was successful, failed or canceled. After that, we created a column using =SUM() function to create a total for the successful, failed and canceled projects in the 'plays' subcategory. Next, we created 3 more calculated columns to determine the proportion of successful, failed and canceled outcomes proportion to the 'goal' grouping's total outcomes. Finally, we graphed our results on a line chart with proportion percentage on the Y-axis, goal grouping on the X-axis and the different outcomes seperated by color.

### Challenges and Difficulties Encountered
One of the challenges I encountered involved the excercise with the COUNTIFS function. Whenever I ran the COUNTIFS function, I couldn't get the sum of all the cells from the COUNTIF function to equal the sum of the kickstarter raw data. The reason was because my range was non inclusive of some numbers. For example, for goals between 10000 and 14999 I used 10000<x<14999 and started the next COUNTIFS on 15000, so if there was any values between 14999 and 15000, they would've been left out. I fixed this by changing range to 10000<=x<15000 to include decimals leading up to 15000.
	 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The first conclusion I draw is that May has the highest number of successful outcomes. The second conclusion I draw is that May also has the highest number of total outcomes overall. You could argue that May only has the highest success rate because it has the highest total, but May also has the highest success rate proportion overall as well. If I were going to launch a theater kickstarter fundraising campaign, I would do it in May.

- What can you conclude about the Outcomes based on Goals?
The first conclusion I draw is that size of goal and success rate are negatively correlated. The number of successful and percentage successful are highest in the lowest goal groupings. This makes logical sense since smaller targets are generally more attaintable. The second conclusion I draw is that the highest success rate and highest number of total projects fall in the 1000 to 4999 goal grouping. If I wanted to have the highest chance of a successful play, I would set the goal somewhere between 1000 and 5000.

- What are some limitations of this dataset?
One limitation of the dataset is that there is only data for 9 different categories. There are many more actual kickstarter categories than the 9 listed. Another limitation is that the currency isn't standardized. This makes analysis difficult since we can't compare across currencies without converting.

- What are some other possible tables and/or graphs that we could create?
We could've created line graphs to show the relationship of backers and success, we didnt use backers for any of these analyses. We also could've created a visualization (most likely another line graph) to compare the average length of a campaign to it's success rate. 
