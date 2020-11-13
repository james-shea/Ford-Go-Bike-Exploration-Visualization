# Udacity Communicate Data Findings Readme for Data Analysis Nanodegree
## by James Shea


## Ford GoBike System Data

Ford GoBike System Data, now known as Bay Wheels, has data available for public use. It is a bicycle sharing program on the West Coast of the USA.
This dataset was found as one of the suggestions in the instructions for this project and downloaded from the link provided.

## Data Cleaning
First, all of the data was downloaded from the link provided and saved in a local folder.
As the data was provided across multiple csv files, these files were then combined into a single csv, which was then loaded as a dataframe.
Next, a copy of this dataframe was made in order to clean the data.
Duplicates were checked but none were found.
Start and end times were converted to datetime type.
User type and bike share for all trip columns were converted to category. 
Ids for the bikes and stations were conveerted to objects instead of floats.
New columns were made for dates/times for later use.
## Exploration
To start, monthly usage of the program was looked at. We can see that March and April were the most popular months.
Then, daily usage was looked at, and we found that weekends had the lowest usage.
Hourly usage exploration showed that usage peaked around 8am and 5pm.
Trip duration tended to be under 10 minutes, with all under 60 minutes.
We also see that most customers are subscribers, with far fewer customers using the program.
## Analysis
Subscribers tended to take shorter trips than customers, and while both had a lot of overlap with each other for start time subscribers also tended to start a little earlier.
Subscribers tended to have much more variance in usage by hour than customers.
Both subscribers and customers had similar patterns of usage across the year by month, with most usage in March and April.
Daily usage had more variance for subscribers than customers.
Subscribers had more usage during the week while customers had more usage on weekends.
Trips tended to last longer on weekends than on weekdays.
Trips lasted longer in summer months (June and July) than other months.
## Multivariate Analysis
Customers tended to have a larger variance in trip length due to the day of the week compared to subscribers with longer trips on the weekend for both groups.
This suggests that subscribers tended to use the bikes for consistent trips, while customers had more inconsistent trips.
One possible explanation for this is that subscribers tended to use the bikes for work and other regular reasons (e.g. shopping) when compared to customers.
Customers may tend to use the bikes for unexpected or less frequent uses such as a fun day riding or a last minute need to travel by bike.
Trip duration also had greater variance for customers than for subscribers due to month.
This provides further support that subscribers tend to have a specific, consistent use for the bikes than customers do.
Finally, customers also had greater variation in trip length based on when the bike trip started.
This provides further evidence that customers have less consistent uses for the bikes.
## Insights
Customers tended to have greater variance in trip length as a consequence of multiple factors, including time the trip start, day of the week, and month of the year when compared to subscribers.
From this, we can infer that subscribers tend to use the bikes for a specific, reoccuring use that occurs on a regular basis.
Further, we can infer that customers tend to use the bikes for less frequent uses, and that customers use bikes for reasons that influenced more by time of day, day of week, and month of year than subscribers.
This suggests that there are two very different use cases based on customer type for the bikes.