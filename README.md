# Kickstarting with Excel

## Overview of Project

This repository contains information about crowd-funded events in different countries. The total goal to be reached is shown as well as the amount raised, the status, day, and category of the event, as well as additional information to analyze.


### Purpose

The "kickStarter" datasheet contains the clean data. The "Text to column" method was used to acquire the subcategories to which each event belongs.
The formula "= Years ()" was used to extract the year in which the funding campaign was carried out to obtain the relationship between the outcome of the project as a function of the month the funding began.

The second analysis was to acquire the number of successful campaigns, and failed campaigns in the "Plays" subcategory according to their goal.


## Analysis and Challenges

The challenging part of this work was trying to sort the clean data in an efficient way to get the desired relationships between the data.
Within my analysis was to create a new column to extract the month of the launch date, and to be able to include it more easily in a pivot table.



### Analysis of Outcomes Based on Launch Date

To obtain the outcome based on its launch date, I had the challenge of obtaining the month of the launch date.
For that I create a new column in the "KickStarter" datasheet and use the formula "= TEXT (S522," mmmm ")" which returns in text the month of the date in cell "S522"

After this use a pivot table to filter the data in the "theater" subcategory and get the relationship between the release date expressed in months and its outcome.

A pivote line chart was used to display the data. 

### Analysis of Outcomes Based on Goals

For the Analysis of Outcomes Based on Goals it was necessary to use the formula "= COUNTIF (" and "= COUNTIFS ("
to "sum" the sample if the cell met the condition.

To achieve this, I had to create a new pivot table to filter the data with the subcategory of "Plays" and organize the columns to show the "Successfull" ones, "Failed" eleven and "canceled" ones and apply the prevoius formula.

### Challenges and Difficulties Encountered

The most important limitation that I found was that the pivot table that orders the data cannot be modified since it would alter the results.

a second challenge was to use the formula "= Counifs (" with two conditionals and a cell as the reference value.


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

    1.- The highest probability for a campaign in the category of "theaters" to occur between the months of May and June.
    73% of the campaigns launched in June were successful.

    2.- The data shows that the worst time to launch a serious campaign in the month of January where only 58% of the campaigns were successful

- What can you conclude about the Outcomes based on Goals?

The category of "Plays" has a very interesting fact and that is that not a single one was canceled.

In addition 387 campaigns (91% of the total) with a goal of between 1000 and 5000 were successful.

While the probability of success in goals greater than 45000 it`s very low. Because only 30% of them where successful. 

- What are some limitations of this dataset?

A very interesting fact to know is the reason for the cancellation of a project, which is a limitation of this dataset, which does not specify the reason why an event was canceled.

- What are some other possible tables and/or graphs that we could create?

You could obtain data from successful campaigns filtered by country, and by goal to estimate the number of successful campaigns based on your goal.

An interesting piece of information would be to know the time it takes to raise funds for a specific successful campaign. With this we could estimate the duration of our deadline
