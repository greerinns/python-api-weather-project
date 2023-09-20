# Python API Weather and Vacation Planning Project

## Introduction

This project is a comprehensive exploration of weather data for over 500 cities located at different distances from the equator. It involves the use of the OpenWeatherMap API and the citipy Python library. The project is divided into two main parts: WeatherPy and VacationPy.

## Part 1: WeatherPy

### Weather Variable vs. Latitude Relationship Visualization

In the first part, we leverage the OpenWeatherMap API to fetch weather data for cities generated using the citipy library. The key visualizations in this section include scatter plots that showcase the relationship between various weather variables and latitude. We explore the following relationships:

1. Latitude vs. Temperature
2. Latitude vs. Humidity
3. Latitude vs. Cloudiness
4. Latitude vs. Wind Speed

### Linear Regression Analysis

In the subsequent step, we conduct linear regression analysis for each of these relationships. We divide the dataset into the Northern Hemisphere (cities with latitudes greater than or equal to 0 degrees) and the Southern Hemisphere (cities with latitudes less than 0 degrees). For each hemisphere, we create scatter plots that incorporate the linear regression line, the regression model's formula, and the corresponding r-values. The specific plots include:

- Northern Hemisphere: Temperature vs. Latitude
- Southern Hemisphere: Temperature vs. Latitude
- Northern Hemisphere: Humidity vs. Latitude
- Southern Hemisphere: Humidity vs. Latitude
- Northern Hemisphere: Cloudiness vs. Latitude
- Southern Hemisphere: Cloudiness vs. Latitude
- Northern Hemisphere: Wind Speed vs. Latitude
- Southern Hemisphere: Wind Speed vs. Latitude

## Part 2: VacationPy

In the second part of the project, we utilize our weather data insights to plan future vacations. This is achieved through the use of Jupyter notebooks, the geoViews Python library, and the Geoapify API.

### City Mapping

We create a map that displays a point for each city in the city_data_df DataFrame. The size of each point corresponds to the humidity level of the respective city.

### Filtering Cities for Ideal Vacation Spots

We narrow down the city_data_df DataFrame to identify cities with maximum temperatures between 21 and 27 degrees Celsius, wind speeds less than 4.5 meters per second, and zero cloudiness.

### Hotel Data Collection

A new DataFrame, hotel_df, is created to store information about selected cities, including the city name, country, coordinates, and humidity level.

### Finding Nearby Hotels

For each city, we utilize the Geoapify API to find the first hotel located within 10,000 meters of its coordinates.

### Adding Hotel Information to City Mapping

To enhance the user experience, we include the hotel name and country as additional information in the hover message for each city on the map.

## Conclusion

This project demonstrates the practical application of Python coding skills for visualizing weather data and planning future vacations. We make use of various Python libraries, including citipy, OpenWeatherMap, geoViews, and Geoapify, to gather, process, and display data. The scatter plots and linear regression analyses help us gain insights into the relationship between weather variables and latitude, while the map visualization showcases the capabilities of the Geoapify API. Overall, this project exemplifies the power of data-driven decision-making and geographical information systems in travel planning.
