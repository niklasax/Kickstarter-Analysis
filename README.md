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

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The first conclusion I draw is that May has the highest number of successful outcomes. The second conclusion I draw is that May also has the highest number of total outcomes overall. You could argue that May only has the highest success rate because it has the highest total, but May also has the highest success rate proportion overall as well. If I were going to launch a theater kickstarter fundraising campaign, I would do it in May.

- What can you conclude about the Outcomes based on Goals?
The first conclusion I draw is that the smaller the goal is, the more likely it is to succeed. 

The second conclusion I draw is that

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
