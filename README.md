## Communicate-Ford-Bike-Data-Findings

This project is divided into two major parts:

- In the first part, I conducted an exploratory data analysis on a dataset Ford GoBike System Data. I used Python data science and data visualization libraries to explore the dataset’s variables and understand the data’s structure, oddities, patterns and relationships. The analysis in this part is structured, going from simple univariate relationships up through multivariate relationships.

- In the second part, I took my main findings from my exploration and conveyed them to others through an explanatory analysis. To this end, I created a slide deck that leverages polished, explanatory visualizations to communicate my results.

## Dataset

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

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
- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)

## Data Wrangling Process

Changed multiple fields that are not in the correct dtype, i.e. start_time, end_time should be datetime type, user_type should be categorical data type.
Added new columns for trip duration in minute, trip start date, trip start hour of the day, Start day, Start week and Start month.
Converted 'start_dayofweek' to category dtype
Converted 'start_month' to category dtype for easy plotting

## Summary of Findings

The number of trips peaked around 8-9am and 4-6pm during a day, there were more trips on work days (Mon-Fri) compared to weekends.
Summer time was the most popular season of a year, likely due to the weather.
There are a lot more subscriber usage than customers overall. The riding pattern varies a lot between subscribers and customers.
Subscribers use the bike sharing system for work commnute thus most trips were on work days (Mon-Fri) and especially during rush hours (when going to work in the morning and getting off work in the afternoon), whereas customers tend to ride for fun in the afternoon or early evenings over weekends. - Subscriber usage peaks out on typical rush hours when people go to work in the morning and getting off work in the afternoon, which strengthened their usage purpose and goal of riding.
Similar pattern was not observed among customers who tend to ride most in the afternoon or early evening for a different purpose than the subscribers.

## Key Insights

- Different habits between the two type of riders are seen from the exploration-

Subscribers use the system heavily on work days i.e. Monday through Friday whereas customers ride a lot on weekends, especially in the afternoon.
Many trips concentrated around 8-9am and 4-6pm on work days for subscribers, yet customers tend to use more in the late afternoon around 5pm Monday to Friday.
The efficient/short period of usage for subscribers corresponds to their high concentration on rush hours Monday through Friday, indicating the use is primarily for work commute.
The more relaxing and flexible pattern of customer use shows that they're taking advantage of the bike sharing system quite differently from the subscribers, heavily over weekends and in the afternoon, for city tour or leisure purpose probably.
