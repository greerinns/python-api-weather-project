# python-api-challenge
## Introduction
This project involves creating a Python script to visualize the weather of over 500 cities of varying distances from the equator. The data is obtained using the OpenWeatherMap API and the citipy Python library. In the first part of the assignment, we create scatter plots to showcase the relationship between weather variables and latitude, and compute linear regression for each relationship. In the second part, we plan future vacations by creating a map visualization using geoViews Python library and Geoapify API.

## Part 1: WeatherPy

### Create Plots to Showcase the Relationship Between Weather Variables and Latitude
In this part, we use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, we create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

### Compute Linear Regression for Each Relationship
In this part, we compute the linear regression for each relationship. We separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). We create a series of scatter plots including the linear regression line, the model's formula, and the r values. We create the following plots:

Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude
## Part 2: VacationPy
In this part, we use our weather data skills to plan future vacations. We use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

### Create a Map that Displays a Point for Every City
We create a map that displays a point for every city in the city_data_df DataFrame. The size of the point is the humidity in each city.


### Narrow Down the city_data_df DataFrame
We narrow down the city_data_df DataFrame to find max temperature lower than 27 degrees but higher than 21, wind speed less than 4.5 m/s, and zero cloudiness.

### Create a New DataFrame Called hotel_df
We create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

### Use Geoapify API to Find the First Hotel Located Within 10,000 Meters of Your Coordinates
For each city, we use the Geoapify API to find the first hotel located within 10,000 meters of the coordinates.

### Add Hotel Name and Country as Additional Information in the Hover Message for Each City on the Map
We add the hotel name and the country as additional information in the hover message for each city on the map.

## Conclusion
This project involves using Python coding skills to visualize weather data and plan future vacations. We use various libraries such as citipy, OpenWeatherMap, geoViews, and Geoapify to obtain and manipulate the data. The scatter plots and linear regression help us to understand the relationship between weather variables and latitude. The map visualization helps us to demonstrate the power of the Geoapify API.
