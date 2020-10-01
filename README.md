# Kickstarting with Excel




## Overview of Project

### Purpose
The purpose of this project was to gain familiarity with Excel by sorting, analyzing, summarizing and visualizing data. In this particular example, we looked at kickstarter data with the ultimate goal of determining if there are certain factors, if any, that make a kickstarter funding campaign successful.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
For this analysis, we wanted to see if there was any correlation between a Theater campaign's launch month and its success. We first took the raw data from the kickstarter tab and added a =YEAR() calculation at the end of the table to display only the year from the date created conversion. We also split 'category' and 'subcategory' into their own columns using the text to columns function. From there, we used the pivot function to filter and summarize our data. The pivot table was filtered to show only 'theater' from the parent category, 'date created conversion' was designated as the rows, 'outcome' was designated as the columns and count of outcomes was used for the values. Finally, we created a line chart from the pivot table with count of outcomes as the Y-axis, the months as the X-axis, and the different outcomes seperated by color.

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
