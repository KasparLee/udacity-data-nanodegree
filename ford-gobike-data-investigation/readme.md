# Ford GoBike Data Investigation
## By Kaspar Lee

**NOTE: In order to run the notebooks, the Ford GoBike trip data must be extracted from `2017-fordgobike-tripdata.csv` first. The file itself could not be uploaded due to it exceeding the 100MB size limit.**


## Dataset

This dataset (downloaded from [here](https://s3.amazonaws.com/fordgobike-data/index.html)) from bicycle sharing service Ford GoBike contains over entries for 519,700 trips made during 2017, with variables relating to both trip data itself (e.g. location info) as well as data on the cyclist/user (e.g. birth year, gender and whether or not they are a subscriber).


## Summary of Findings

- **Univariate Exploration** - I found that the trip duration follows a right skewed distribution, however when plotting on a logarithmic scale, it follows a normal distribution. Additionally, the start/end times of journeys are bimodally distributed, with peaks during the morning and evening "rush hour". The most popular stations are all in popular locations in San Fransisco, and far more trips were made by subscribers than one-off users. The majority of riders are aged under 40 years old, and there are very few journeys made by over 70s. Finally, males made far more trips than females or other genders.

- **Bivariate Exploration** - The distribution of trip durations for subscribers was centered around 500 seconds (8m 20s), with little variation, whereas the distribution for one-off customers was less peaked and wider (larger range of durations). The number of trips for customers increases during the day until late afternoon, before staring to drop off, whereas for subscribers there are 2 distinct peaks during rush hour time where the most trips are made. Finally, over the age of 25, age has little impact on trip duration.

- **Multivariate Exploration** - The average duration of trips of subscribers doesn't seem to vary with the time of day the trip starts. However for trips made by customers, early morning (before 5am) trips tend to be the longest in duration, with 8am trips being the shortest. Furthermore, the number of trips made per month has been consistency increasing, and at essentially the same rate for all genders.


## Key Insights for Presentation

How trip durations vary based on whether a user is a subscriber or not and time of day when staring trip, as this is useful to visualise how long bikes are in use for based on these variables. Additionally, looking at the total number of trips per month and how this changes over time would be useful to examine how demand for Ford GoBikes is changing.