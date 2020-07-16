**Python API Homework - What's the Weather Like?**

**Background**

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: "Ofcourse, It gets hotter..."

But, if pressed, how do we prove it?

![](Images/Image1.png)

**Part I - WeatherPy**
In this example, I be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a few Python libraries, the OpenWeatherMap API,and a representative model of weather across world cities.

First objective wass to build a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude
After each plot add a sentence or too explaining what the code is and analyzing.

Next objective was to run a linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude
After each pair of plots explain what the linear regression is modelling such as any relationships you notice and any other analysis you may have.

**The final notebook:**

Randomly selected over 500 unique (non-repeated) cities based on latitude and longitude.
Performed a weather check on each of the cities using a series of successive API calls.
Included a print log of each city as it's being processed with the city number and city name.


**Part II - VacationPy**

This part involved usin skills in working with weather data to plan future vacations. Used jupyter-gmaps and the Google Places API for this part of the assignment.

Created a heat map that displays the humidity for every city from the part I of the homework.

![](Images/Image2.png)

Started off by narrowing down the DataFrame to find the ideal weather condition. For example:

A max temperature lower than 80 degrees but higher than 70.

Wind speed less than 10 mph.

Zero cloudiness.

Dropped any rows that didn't contain all three conditions and made sure the weather Was ideal.

Note: Limited the number of rows returned by the API requests to a reasonable number.

Used Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

![](Images/Image3.png)


