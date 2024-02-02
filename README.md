# python-api-challenge
### Part 1: WeatherPy
#### Use Python requests, APIs, and JSON traversals to analyze weather data
I created a Python script to visualize weather data of over 500 cities at different distances from the equator

  1. In order to create the list of cities I created a set of random latitude and longitude combinations, used the `citipy` library to find the nearest city, and stored the name of the city and the latitude and longitude in a list. I used `len()` to confirm the list of cities was longer than 500, it was 626.
  2.  I used the `OpenWeatherMap API` to retrieve weather data from the cities list generated in the starter code and created a series of scatter plots to showcase the following relationships:
    - Latitude vs. Temperature
    - Latitude vs. Humidity
    - Latitude vs. Cloudiness
    - Latitude vs. Wind Speed
  3. I computed the linear regression for each relationship, and included the linear regression line, the model's formula, and the r values.
  - The following were created:
    - Northern Hemisphere: Temperature vs. Latitude
    - Southern Hemisphere: Temperature vs. Latitude
    - Northern Hemisphere: Humidity vs. Latitude
    - Southern Hemisphere: Humidity vs. Latitude
    - Northern Hemisphere: Cloudiness vs. Latitude
    - Southern Hemisphere: Cloudiness vs. Latitude
    - Northern Hemisphere: Wind Speed vs. Latitude
    - Southern Hemisphere: Wind Speed vs. Latitude

### Part 2: VacationPy
#### Use the `Geoapify API` and the `geoViews` Python library to create map visualizations
  1. I imported the list of cities stored in the `cities.csv` file from Part 1 and stored the data in a dataframe.
  2. I used the `gmaps` library to create a heatmap that displayed each city and the humidity of each city determined the size of the marker.
  3. I created a new dataframe that included only cities where the maximum temperature was below 27 and above 21, a humidity below 70%, no cloudiness, and wind speed below 4.5 mph.
  4. I added a `Hotel Name` column and used `gmaps` to search hotels within 10000 meters from each city and stored the closest hotel to the latitude and longitude set for each city.
  5. I created a heatmap with the locations with my ideal weather with hover messages that showed where the hotels are, and created a display box showing the city name, hotel name, and country.
