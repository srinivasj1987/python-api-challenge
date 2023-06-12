# Python API Project - What's the Weather Like?

# Background

I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator.

# Part I - WeatherPy

I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. 

## Observation

- Southern Hemisphere climates tend to be slightly milder than those at similar latitudes in the Northern Hemisphere. This is because the Southern Hemisphere has significantly more ocean and much less land; water heats up and cools down more slowly than land.

- "Highest temperature is found at 0 latitude and as the latidude increases or decreases, temperature drops. This happens as equatorial region receives sunlight straight with less or no angle due to curvature shape of earth.\n",

- "Latitude doesn't have a strong iinfluence on wind speed. The speed of the wind is controlled by the strength of the air pressure gradient, the stronger the pressure gradient the higher the wind speed. "

## Objectives

My first objective is to build a series of scatter plots to showcase the following relationships:

- Temperature (F) vs. Latitude

Highest temperature is found at 0 latitude and as the latidude increases or decreases, temperature drops.

- Humidity (%) vs. Latitude

  Polar regions have lower humidity and as latitude gets higher,humidity gets higher in southern hemisphere.

- Cloudiness (%) vs. Latitude


Cloudiness data is widely spread across the latitude.

- Wind Speed (mph) vs. Latitude


  Wind speed data is widely spread across the latitude.

My second objective is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

- Northern Hemisphere - Temperature (F) vs. Latitude


The r-squared is : -0.75
There is a strong negative correlation between latitude and max temperature for northern hemisphere.

- Southern Hemisphere - Temperature (F) vs. Latitude

The r-squared is : 0.85
There is a strong positive correlation between latitude and max temperature for southern hemisphere.

- Northern Hemisphere - Humidity (%) vs. Latitude

The r-squared is : 0.04
There is a weak positive correlation between latitude and humidity for northern hemisphere.

- Southern Hemisphere - Humidity (%) vs. Latitude

The r-squared is : 0.06
There is a weak positive correlation between latitude and humidity for southern hemisphere.

- Northern Hemisphere - Cloudiness (%) vs. Latitude

The r-squared is : 0.007
There is a weak positive correlation between latitude and cloudiness for northern hemisphere.

- Southern Hemisphere - Cloudiness (%) vs. Latitude

The r-squared is : 0.14
There is a weak positive correlation between latitude and cloudiness for southern hemisphere.

- Northern Hemisphere - Wind Speed (m/s) vs. Latitude

The r-squared is : -0.08
There is a weak negative correlation between latitude and windspeed for northern hemisphere.

- Southern Hemisphere - Wind Speed (mph) vs. Latitude

The r-squared is : -0.283
There is a weak negative correlation between latitude and wind speed for southern hemisphere.

My final notebook must:

- Randomly select **at least** 500 unique (non-repeat) cities based on latitude and longitude.
- Perform a weather check on each of the cities using a series of successive API calls.
- Include a print log of each city as it's being processed with the city number and city name.
- Save a CSV of all retrieved data and a PNG image for each scatter plot.

# Part II - VacationPy

Now I want to use my skills in working with weather data to plan future vacations. I used jupyter-gmaps and the Google Places API.

- Create a heat map that displays the humidity for every city from the part I of the project.

- Narrow down the DataFrame to find my ideal weather condition. For example:

  - A max temperature lower than 27 degrees but higher than 21
  - Wind speed less than 4.5 m/s
  - Zero cloudiness


  ## To run the code:

  - Install citypy in your python environment (https://pypi.python.org/pypi/citipy)
  - Save OpenWeatherMap API Key (https://openweathermap.org/) as 'weather_api_key'
  - Google API Key (https://console.developers.google.com/getting-started) as 'g_key'
  - Create API Keys and store it in the 'api_keys.py' file before running the Jupyter notebooks.
