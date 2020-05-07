# API Challenge: Weather Research
What's the weather like as we approach the equator?

Hotter of course. Lets prove it. 

## Observations

1. City Latitude vs Max Temperature(F), for both hemisphere's, display the trend we are seeking. The closer to the equator (lat = 0), the hotter it gets. As the Northern Hemisphere is entering the Summer season, we can see the Latitude referencing the Northern Hemisphere is as hot as the equator. The R-Value squared is .77 for northern which is a good correlation to reference as we are looking to be closer to 1. The southern value is at .58. A little in the middle but as the season changes, temperatures may fluctuate.

2. City Latitude vs. Humidity shows a .56 correlation on the Northern Hemisphere. Summer will display more humid temperatures over winter. Southern Hemispher may be lower-- which is at .004 correlation. Although Northern Hemispherr is at .56, City Lat vs. Humidity does not look like a good correlation. 

3. City Lat vs Cloudiness/Windy City did not have much a solid correlation on either side of the hemisphere. 


### Libraries & API:
* CitiPy, Numpy, Pandas, time, SciPy, requests, math, json, requests
* Weathermap API


### WeatherPy

Visualize the weather of 500+ cities across the world of varying distance from the equator. 500+ cities will be generated randomly. The max temperature, humidity, cloudiness, and wind speed will be captured. Included is a print log of each city as it's being processed with the city number and city name. Data will be displayed in a series of scatter plots showcasing the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Data is saved to a CSV. Scatter plots are saved as a PNG image.

Run linear regression on each relationship, only this time separating them into Northern Hemisphereand Southern Hemisphere:

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

#### Additional Information: 

Optimized creating linear regression plots by creating a function. The function accepted the first relationships created and generates the linear regressions for Northern and Southern hemisphere comparisions.


### VacationPy

### Additional Libraries & API:
* Google Places API 
* Gmaps

Create a heat map that displays the humidity for every city from WeatherPy. Afterwards, narrow down the DataFrame to find the ideal weather condition listed below:

* A max temperature lower than 80 degrees but higher than 70.
* Wind speed less than 10 mph.
* Zero cloudiness.

Other conditions: Dropped any rows that don't contain all three conditions. Next, Using Google Places API, find the first hotel for each city located within 5000 meters of coordinates.

Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.


