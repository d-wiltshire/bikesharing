# bikesharing

## Overview

The goal of this exercise is to analyze NYC Citibike data from August 2019 and to describe various metrics using visualizations in Tableau. The use case for these visualizations is a fictitious pitch to a body of investors to create a similar bikeshare program in Des Moines, Iowa. The visualizations depict information like the total number of rides broken down by gender, trip duration, time of day, etc., in order to help the investors make an informed decision. 

The resulting Story <a href="https://public.tableau.com/app/profile/david1924/viz/August2019CitibikeUsage/August2019CitibikeUsage">can be viewed on Tableau Public here</a>.


### Note
The data used here were downloaded from the Citibike website. The "trip duration" data were originally stored with the "integer" datatype. This column was converted to a "datetime" datatype using Python and Pandas in Jupyter Notebook before use in the graphs presented here. This Python code is included in this repository.


## Results

The Tableau Story contains seven visualizations:

### Checkout Times for Users (i.e., checkout durations)
A graph of the duration of time that bikes are checked out for all riders

![tableau1](https://user-images.githubusercontent.com/100863488/171236581-3483720f-9951-4429-a904-275d9f320aaa.png)

* The results show that the vast majority of riders checked out a bike for less than an hour.

---



### Checkout Times by Gender
A graph of the duration of time that bikes are checked out for all riders, broken down by gender

![tableau2](https://user-images.githubusercontent.com/100863488/171236614-aefb712a-31a8-41d1-bde1-5e92e881bd99.png)

* The results show that the trends for ride duration among the genders are similar. In addition, these results show that the majority of rides are taken by men.

---



### Trips by Weekday per Hour
A graph of the number of bike trips by weekday for each hour of the day as a heatmap

![tableau3](https://user-images.githubusercontent.com/100863488/171236675-00003e65-0798-42b6-ba35-35e654cbfbbc.png)

* This heatmap shows the most frequent concluding times for trips. Most trips were taken during morning and afternoon weekday rush hour.

---



### Trips by Gender (Weekday per Hour)
A graph of the number of bike trips by weekday for each hour of the day as a heatmap, divided by gender into multiple heatmaps

![tableau4](https://user-images.githubusercontent.com/100863488/171236717-03a4af4c-0d09-47dd-a03a-156093f5ffc7.png)

* This heatmap shows the most frequent concluding times for trips, broken down by gender. Most trips were taken during morning and afternoon weekday rush hour, and the trends between men and women are very similar.

---



### Trips by Gender, by Weekday, by User Type
A heatmap that shows the number of bike trips broken down by gender for each day of the week by each user type (i.e., whether the user is a non-subscriber or a subscriber)

![tableau5](https://user-images.githubusercontent.com/100863488/171242037-4d7e6304-da31-46a0-8fab-c04a8e044de7.png)

* Most rides were taken by male subscribers, especially toward the end of the week (Thursday-Saturday).

---



### Customers by User Type
A pie chart depicting the percentages of users who are customers and who are subscribers


![tableau6](https://user-images.githubusercontent.com/100863488/171236809-d5439873-ebc7-481c-8e7f-bba3e3269386.png)

* The results show that the vast majority of rides were taken by subscribers.

---
 
 

### Bike Usage by Hour
A bar chart showing the hours of the day when rides were initiated (trip start time)


![tableau7](https://user-images.githubusercontent.com/100863488/171236829-497d25de-a196-46d6-8e5d-ca4c643d6779.png)

* This bar chart shows the most frequent times for users to initiate bike trips. The heaviest usage falls during rush hour times (7-10AM and 5-8PM).

---



## Summary

The results show that the majority of NYC users in August 2019 were subscribers and male, and the highest use periods were on weekdays during morning and evening rush hours. This suggests that the majority of users in NYC are not tourists but residents who rely on Citi Bike for a daily commute. Therefore, in order to determine whether a similar bikesharing model would work well for a city like Des Moines, additional information regarding tourism dollars would be less helpful than information like 1) the population density of Des Moines and proximity between residential areas and commercial areas, 2) a map of Des Moines indicating which streets have bike lanes or where bikes are permitted on sidewalks, or 3) the types of industries in Des Moines and whether places of employment tend to be located in the downtown area.



### Additional suggestions for future visualizations

We could use the current dataset to create additional helpful visualizations to assist our investors:

* Because start and stop locations are included in the dataset, we could create a visualization regarding the average trip length (in miles/kilometers). If places of interest in Des Moines are much more distant from one another than the average trip length in NYC, Des Moines might not be a good candidate for investment.
* Because birth year is included in the dataset, we could create a visualization regarding the ages of users and their relative usage rates. If the most frequent age ranges of users in NYC are not well represented among the demographics in Des Moines (for example, if the most frequent users in NYC are men in their 20's, and if NYC has a far higher population of men in their 20's than Des Moines), there might not be as solid a market in Des Moines as in NYC.

