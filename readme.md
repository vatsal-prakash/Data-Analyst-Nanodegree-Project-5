# Ford GoBike Data Exploration


## By Vatsal Prakash

## About the Project

This project consisted of two parts and laid emphasis on data visualization techniques in the data analysis process. In the first part, two of Python's libraries seaborn and matplotlib were used to explore Ford GoBike data for the month of April 2019.
Firstly the exploration started with creating visualizations for single variables (univariate exploration) and moved to bivariate and multivariate exploration of the data.

For the second part of the project, a short presentation was created to convey our data findings to an audience. The primary method of conveying the findings was through transforming the visualizations created in part I of the project into polished, explanatory visualizations.


### Dataset



This dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

Each trip is anonymized and includes:

- Trip Duration (seconds)
- Start Time and Date
- End Time and Date
- Start Station ID
- Start Station Name
- Start Station Latitude
- Start Station Longitude
- End Station ID
- End Station Name
- End Station Latitude
- End Station Longitude
- Bike ID
- Bike share for all trip
- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)


**The following issues were found and resolved:**

- start_station_id, end_station_id and bike_id are not string types
- start_station_id, start_station_name, end_station_id, end_station_name have some null values
- start_time and end_time is not a datetime object
- user_type and bike_share_for_all_trip columns are not categorical types

## Summary of Findings 

Through the exploration of the data, we were able to pose some questions. They were as follows:

- What are the most popular and the least popular start and stop stations?
- Which bike is most frequently used?
- How many users are there in each catergory type?
- What is the proportion of bike share for all trip?
- Which day had most and least number of starting trips?
- What is the most common hour of the day when the trips starts?

### At univariate exploration level we found that 
- most common start and stop station is San Francisco Caltrain Station 2 
- bike ids with number 67, 58 and 15 were most frequently used 
- 85% of the user type are subscribers and only 15% is customer type 
- Tuesday had the highest number of trips starting on the day while Sunday had the least 
- Most common time for the start of the trip was around 8 am or 5 pm


### At bivariate exploration level we found that 

- There was very less difference between latitudes and longitudes suggest most of the trips were short 
- Most common start time for the trip was around 8 am or 5 pm on weekdays but on weekends it ranged from 12 pm to 6 pm
- Average duration of the trip increased on 6th, 13th, 20th and 27th of the month


### At multivariate exploration level we found that 

Some variables had a high positive or negative correlation

**High Positive Correlation**
- start station longitude vs end station longitude
- start station latitude vs end station latitude

**High Negative Correlation**
- start station latitude vs start station longitude
- start station longitude vs end station latitude
- end station longitude vs end station latitude
