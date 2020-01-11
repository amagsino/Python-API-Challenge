# Python API Challenge - What's the Weather Like?

## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter..."_

But, if pressed, how would you **prove** it?

## WeatherPy

In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

Your objective is to build a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Your final notebook must:

* Randomly select **at least** 500 unique (non-repeat) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save both a CSV of all data retrieved and png images for each scatter plot.

As final considerations:

* Create a new GitHub repository for this project called `API-Challenge` (note the kebab-case). **Do not add to an existing repo**
* You must complete your analysis using a Jupyter notebook.
* You must use the Matplotlib or Pandas plotting libraries.
* You must include a written description of three observable trends based on the data.
* You must use proper labeling of your plots, including aspects like: Plot Titles (with date of analysis) and Axes Labels.
-----
## Observations Based on Data
1. There is a correlation between latitude and temperature. As one approaches the equator, which is represented by 0 Degrees Latitude, the temperature becomes significantly warmer. However, the weather peaks at -20 Degrees Latitude, rather than at 0 Degrees Latitude, which may be due to obliquity, the angle of tilt of the Earth's axis of rotation.
2. In regards to the date that the data was collected, it is much warmer in the southern hemisphere, which is represented by negative Degrees of Latitude compared to the northern hemisphere represented by positive degrees of Latitude. It is currently Fall season in the northern hemisphere and Summer season in the southern hemisphere. The highest recorded temperature in the southern hemisphere is about 100 Degrees F, while the lowest recorded temperature in the northern hemisphere is about -40 Degrees F.
3. Wind speed is generally between 0 and 15mph regardless of latitude, with some few points beyond that range. The highest recorded wind speed of about 50mph.
