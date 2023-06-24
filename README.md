# python-api-challenge
Module 6 HW challenge python API challenge
By Emanuel Emahazion

This data analysis project was based on weather data to look at suitable cities based on geographic and weather data, using APIs.

The APIs used:
* OpenWeatherMap API 
* Geoapify’s API

WEATHER ANALYSIS

We used the weather data to pull hundreds of random coordinates, and then pull the nearest locations, and from there pull the city/country name, and then weather information such as humidity, max temperature(for a specific time of the year), wind speed, cloudiness, etc.

From there we plotted to show visually what we perceived to be true as far as the weather being hotter closer to the equator (as shown in one of the linear regressions for the northern hemisphere below)








We did not see Cloudiness, Wind Speed or Humidity show any strong correlation with being close to the equator, as we had weak correlations.









VACATION ANALYSIS

From the weather analysis we got a csv created with weather info and we try to deduce ideal vacation spots based on weather preferences.

Using the humidity data, we created an interactive weather dashboard to look at locations on a map and there humidity levels via the size of the dots plotted(as seen below):










From the hundreds of cities in the data frame from the weather analysis, we filter to a new dataframe with the city, country, coordinate and humidity only and then further wittle it down with ideal weather conditions. As for myself I selected a humidity of less than 60 and max temperature less than 20 celsius. Im not really a beach person, or hot weather admirer, hence my choices. Also, my parents homeland of Eritrea has these specific attributes, so I wanted to make sure the capital city of Asmara was in the filtered list.


 


I then used the Geoapify API to find the nearest hotel to the specific coordinates in the filtered list. I added more information to the hvplot interactive map dashboard, so that when you hover over a coordinate, you can now see the country and hotel information (as seen below with my parents homeland):


 
     We concluded there were only 14 cities with the specifications I asked for. Out of those 14, only half of them have a hotel within 10,000 meters of the coordinates with my ideal weather. So of course, of the 7 options, I would choose my homeland’s city of Asmara, and stay at Crystal Hotel ???? ???????. Bon Voyage.
