# bikesharing

## Overview

The goal of this exercise is to analyze NYC Citibike data from August 2019 and to describe various metrics using visualizations in Tableau. The use case for these visualizations is a fictitious pitch to a body of investors to create a similar bikeshare program in Des Moines, Iowa. The visualizations depict information like the total number of rides broken down by gender, trip duration, time of day, etc., in order to help the investors make an informed decision. 

The resulting Story <a href="https://public.tableau.com/app/profile/david1924/viz/August2019CitibikeUsage/August2019CitibikeUsage">can be viewed on Tableau Public here</a>.


### Note
The data used here were downloaded from the Citibike website. The "trip duration" data were originally stored with the "integer" datatype. This column was converted to a "datetime" datatype using Python and Pandas in Jupyter Notebook before use in the graphs presented here. This Python code is included in this repository.


## Results

The Tableau Story contains seven visualizations:

* Checkout Times for Users (i.e., checkout durations): a graph of the duration of time that bikes are checked out for all riders
  - The results show that the vast majority of riders checked out a bike for less than an hour.
* Checkout Times by Gender: a graph of the duration of time that bikes are checked out for all riders, broken down by gender
  - The results show that the trends for ride duration among the genders are similar. In addition, these results show that the majority of rides are taken by men.
* Trips by Weekday per Hour: a graph of the number of bike trips by weekday for each hour of the day as a heatmap
  - This heatmap shows the most frequent concluding times for trips. Most trips were taken during morning and afternoon weekday rush hour.
* Trips by Gender (Weekday per Hour): a graph of the number of bike trips by weekday for each hour of the day as a heatmap, divided by gender into multiple heatmaps
  - This heatmap shows the most frequent concluding times for trips, broken down by gender. Most trips were taken during morning and afternoon weekday rush hour.
* Trips by Gender, by Weekday, by User Type: a heatmap that shows the number of bike trips broken down by gender for each day of the week by each user type (i.e., whether the user is a customer or a subscriber)
  - This heatmap shows the number of rides per weekday, broken down by day, gender, and user type (non-subscriber or subscriber). Most rides were taken by male subscribers.
* Customers by User Type: a pie chart depicting the percentages of users who are customers and who are subscribers
  - The results show that the vast majority of rides were taken by subscribers.
* Bike Usage by Hour: a bar chart showing the hours of the day when rides were initiated (trip start time)
  - This bar chart shows the most frequent times for users to initiate bike trips. The heaviest usage falls during rush hour times (7-10AM and 5-8PM).



## Summary

The results show that the majority of NYC users in August 2019 were subscribers and male, and the highest use periods were on weekdays during morning and evening rush hours. This suggests that the majority of users in NYC are not tourists but residents who rely on Citibike for a daily commute. Therefore, in order to determine whether a similar bikesharing model would work well for a city like Des Moines, additional information regarding tourism dollars would be less helpful than information like 1) the population density of Des Moines and proximity between residential areas and commercial areas, 2) a map of Des Moines indicating which streets have bike lanes or where bikes are permitted on sidewalks, or 3) the types of industries in Des Moines and whether places of employment tend to be located in the downtown area.



### Additional suggestions for future visualizations

We could use the current dataset to create additional helpful visualizations to assist our investors:

* first
* second

