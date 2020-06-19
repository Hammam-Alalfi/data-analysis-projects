# Ford GoBike System Data Exploration

## by Hammam Al-Alfi


## Dataset

The dataset contains informations about individual rides made in a bike-sharing system covering the greater San Francisco Bay area on 2018.
The informations includes regarding 1863721 bike-rides as follows:
> The starting and ending station of the trip and thier coordinates.
> The duration of the trip .
> The date and time of the start and end of the trip.
> The user type (Customer or Subsecriber).
> If the member is enrolled in Bike Share For All program (Yes or No).
> A derived-distance-column that gives the shortest distance on the surface of an ellipsoidal model of the earth between the start and end station.
The source of the data set [here](https://www.lyft.com/bikes/bay-wheels/system-data)
The source of San Francisco geojson file that has the boundaries of the neighborhoods of San Francisco [here](https://data.sfgov.org/Geographic-Locations-and-Boundaries/Planning-Neighborhood-Groups-Map/iacs-ws63)
I did some wrangling on my dataset as follows:
> Combining the 12 CSVs files of the months of 2018 into one master dataframe
> Deriving a column called distance from the coordinates of the start and the end stations of each trip that contains values that gives the shortest distance on the surface of an ellipsoidal model of the earth between the start and end station.
>Converting the duration column from string type to timedelta and converting the start_time and end_time from string type to datetime type.
> Getting geoseries instances for the coordinates of the start and end station.
> Getting a two bolean columns (sf_start,sf_end) that shows if the start station or the end station are inside San Francisco.

## Summary of Findings

> The main goal for me was to study what affects the duration of the trip so i started my exploration plotting the distribution of the duration and the reast of the features that i thought might do something with my main feature of interest.
> doing transformation and rescaling to get  the to know  the proper distribution of the distance and duration
> i plotted the distribution of the unique bikes trips count but i chose not to use it in my presention cause it seems that it makes no scence 
>
## Key Insights for Presentation

> The key insights were to show:
>> how the distribution of other variables like weekdays trips and day hours trip differs when they are related to the duration
>> to discuss the relation between the distance and  the duration.
>> how the user type related to the duration of the trip 
>>





