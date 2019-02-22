# Ford_Go_Bike
### by Subaru Goto

This is a part of Udacity Nanodegree project. This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. * This is important to note that as there is no user id information. Therefore, many observations can stem from the same users.
<p></p>
Programming language: Python
Time frame: January 2017 to December 2018.
Module: numpy, pandas, matplotlib, seaborn, glob and folium

## Data structure
There are 2383421 observations in total and 16 columns.

### Variables
Trip Duration (seconds)
Start Time and Date
End Time and Date
Start Station ID
Start Station Name
Start Station Latitude
Start Station Longitude
End Station ID
End Station Name
End Station Latitude
End Station Longitude
Bike ID
User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
Member Year of Birth
Member Gender
bike share for all trip

Reference https://www.fordgobike.com/system-data

## Data wrangling
I downloaded 2 data sets which are from 2017 and 2018.
I have merged the 2 data sets into one data frame. I converted trip duration in second into trip duration in minute. So that it is easier to handle with. Moreover, member year of birth is converted to age by subtracting the value from 2018. A start time and date column is split into time and date columns. A weekday column is made out of the date column.

<strong>Short summary</strong>

About 74 % of Ford Go-bike users are male. More than 80% of users are holders of either monthly or yearly passes. Age distribution is skewed, most users around the age of 30. 75% of users ride a shared bike less than 15 minutes with a median of about 10 minutes. The users without any memberships have a higher average duration per trip, which is about 35 minutes. Whilst subscribers use this service more frequently on the weekdays, non-members tend to use it more on weekends. Most frequently used times during a day for subscribers are around 8-10 am and 17-19 pm. It suggests that many pass-holders may use this service for the purpose of commute. However, there is no effect for non-members. The data also implicates that over time non-members trip duration tends to decrease. Pass-holders use this service more frequently over time. It would be interesting to see any correlation between weather or temperature and usage duration per trip and usage counts.  

<strong> Research questions</strong>

In this analysis I am going to find any user behavioral trends from data set.
<ul>
<li>What kind of people are using this service?</li>
<li>How long do people use this service per trip</li>
<li>when do people use this service?</li>
<li>What kind of changes can be seen over time?</li>
</ul>
