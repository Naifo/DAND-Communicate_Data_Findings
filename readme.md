# Ford GoBike Data Exploration
## by Naif Alsofyani


## Dataset

> [Bay Wheels](https://en.wikipedia.org/wiki/Bay_Wheels) (previously know as Ford GoBike) is a regional public bike-sharing system in the San Francisco Bay Area. And it is the first regional and large-scale bicycle sharing system deployed in California and on the West Coast of the United States. It was established in 2013, and after the acquisition by [Lyft](https://en.wikipedia.org/wiki/Lyft), the system is expected to have 7,000 bicycles around 540 stations in San Francisco, Oakland, Berkeley, Emeryville, and San Jose.

**Data wrangling process**
* fixed multiple fields that are not in the correct dtype, i.e. start_time, end_time should be datetime type, user_type and member_gender should be categorical data type, etc

* added new columns for trip duration in minute, trip start date in yyyy-mm-dd format, trip start hour of the day, day of week and month

* added a new column calculating riders' age from 'member_birth_year'
* filtered out outlier ages 
* filtered out outlier trip records where the duration was very long

## Summary of Findings

> There are significantly more male users, and most of them are subscribers around the age of 25-40 years
>
>Subscribers tend to use the service more than customers do. The riding habit varies between subscribers and customers. Subscribers use the bike-sharing system for work thus, most trips were on workdays and especially during work hours, whereas customers tend to ride on weekends and take longer rides overall.

## Key Insights for Presentation

> In general, younger people tend to use bikes for a longer duration. The short ride duration for subscribers on workdays during work hours showed a pattern that they tend to take bikes for work. The other pattern of customer use shows that they're taking advantage of the bike-sharing system quite different from the subscribers, longer times and more rides on weekends, for having fun rides around the city probably.