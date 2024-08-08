# python-api-challenge
Module 6 API Challenge

## Part 1: WeatherPy
In WeatherPy, we aim to visualize the weather of over 500 cities of varying distances from the equator. The project uses the citipy library to determine city locations based on geographic coordinates and the OpenWeatherMap API to retrieve current weather data.

## Steps
Generate Random Geographic Coordinates: The starter code helps generate random geographic coordinates and find the nearest city for each coordinate.
Retrieve Weather Data: Use the OpenWeatherMap API to get weather data for each city.
Create Scatter Plots:
Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed
Compute Linear Regression: Separate the data into Northern and Southern Hemispheres and compute linear regressions for each of the relationships mentioned above. Include the linear regression line, formula, and r2 values in the plots.

## Results
Scatter plots displaying the relationship between latitude and various weather parameters.
Linear regression analysis to explore

## Part 2: VacationPy

In VacationPy, we leverage our weather data skills to plan future vacations. This part involves using Jupyter notebooks, the hvplot.pandas library, and the Geoapify API to create map visualizations and identify ideal vacation spots based on specific weather conditions.

## Steps
Create an Interactive Map:

Display a point for every city in the city_data_df DataFrame.
The size of the point represents the humidity in each city.

Filter for Ideal Weather Conditions:
Define ideal weather criteria (e.g., max temperature between 21°C and 27°C, wind speed less than 4.5 m/s, and zero cloudiness).
Narrow down the city_data_df DataFrame to include only cities that meet these criteria.

Find Hotels Using Geoapify API:
Create a new DataFrame hotel_df to store city, country, coordinates, and humidity.
For each city in hotel_df, use the Geoapify API to find the first hotel located within 10,000 meters of the city's coordinates.
Add the hotel's name to the hotel_df DataFrame.

Enhance the Map with Hotel Information:
Update the map to include hotel names and countries in the hover messages for each city.

## Results
City Humidity Map: An interactive map displaying points for each city, with the size of the points representing the humidity.
Filtered Cities Map: An interactive map showing cities that meet the defined ideal weather conditions.
Hotel Information Map: An enhanced map that includes hotel names and country information in the hover messages for cities with ideal weather conditions.

## Usage

To view the interactive maps locally:
Run the Jupyter notebooks (WeatherPy.ipynb and VacationPy.ipynb) to generate the visualizations.
Export the notebooks as HTML files if needed for sharing or presentation.

By following these steps, you'll be able to visualize and analyze weather data to identify ideal vacation spots and nearby hotels, using Python and various data visualization libraries.