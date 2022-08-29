# python-api-challenge

 So in this project I try to prove that the weather is hotter when your closer to the equator. I try to answer this by using `API's`.
 I use the `API` from `OpenWeatherMap` and also a `Google API`. The first project was to collect data from more than 600 cities 
 to observe the weather patterns including Temperature, Humidity, Cloudiness and Wind speed this project was called `WeatherPy`
 
 ## WeatherPy
 In this project I took the data I retrieved through the `OpenWeatherMap` API and created a dataframe so I can plot with and made 
 sure to save my dataframe as a .csv file and comment out my API call. I used the data in the save csv file to plot some data by first
 dropping all the cities with an Humidity 100 and above and then  made a series of plots that showcased the following relationships:
 
- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude
 
 
 
 Then I divided the data into `Northen` and `Southern` hemispheres all `Northern Hemisphere` data had a Latitude  greater than or 
 equal to 0 and the `Southern Hemisphere` had a Latitude lower than 0. Once I had the data seperated into north and south I began 
 computing the linear regression for each of the relationships:
 
- Northern Hemisphere - Temperature (F) vs. Latitude
- Southern Hemisphere - Temperature (F) vs. Latitude
- Northern Hemisphere - Humidity (%) vs. Latitude
- Southern Hemisphere - Humidity (%) vs. Latitude
- Northern Hemisphere - Cloudiness (%) vs. Latitude
- Southern Hemisphere - Cloudiness (%) vs. Latitude
- Northern Hemisphere - Wind Speed (mph) vs. Latitude
- Southern Hemisphere - Wind Speed (mph) vs. Latitude

Now that we know and have proof that being closer to the equator is hotter, My second project helps us plan for a vacation by using 
Google API to request and pull a heat map with every city used in the WeatherPy project. this project is called VacationPy 

## VacationPy
In this project I used the data from WeatherPy and created a heatmap then I went ahead and narrowed down from 600 plus by ideal 
weather conditions that were:

- A max temperature lower than 80 degrees but higher than 70.
- Wind speed less than 10 mph.
- Zero cloudiness.

with these criterias i was able to narrow it down to 14 cities and then I used the Google place API to search within a 5000 meter 
radius and plotted the `Hotel Name`, `City`, and `Country`.
