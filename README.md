# Module 6 Challenge: Analysis of Weather and Vacation Spots Using APIs
The purpose of this challenge is to use APIs from two different sites to perform an analysis and a query. 
The first part of this challenge involves OpenWeatherMapAPI and analyzes how various weather metrics change with latitude. The results are displayed in various scatterplots, which compare the Northern and Southern Hemispheres.
The second part of this challenge involves using Geoapify API to perform a query, in order to find hotels in a given desirable climate.

## WeatherPy
The first part of this challenge is to use OpenWeatherMap API to retrieve the following city and weather data:
* city name
* country
* current date
* latitude
* longitude
* maximum temperature
* humidity
* cloudiness
* wind speed

From the data pulled, four scatterplots were created, comparing the maximum temperature, humidity, cloudiness, and wind speed to latitude. Next, the data was split into Northern and Southern Hemisphere and 8 more scatterplots created, each fit with a linear regression line to display the strength of the relationship.

## VacationPy
The second part of this challenge is to use the city dataframe created above to plan a vacation based on the following weather conditions:
* A maximum temperature of between 21 and 27 degrees Celsius
* A wind speed less than 4.5 m/s
* Zero cloudiness
  
From the above conditions, a new dataframe was created with each city that fits these requirements, and the Geoapify API was
used to find the first hotel located within 10,000 meters of each city's coordinates. If a hotel was found, its name and country
was added to the dataframe.
