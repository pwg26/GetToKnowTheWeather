Get to know the weather:


Introduction:
This repository contains a weather forecaster. It works by taking a user input for a given location, then plugging that input into a series of api ajax calls which pulls weather data to ultimately populate the content of the forecast. This forecaster also saves previous user imputes which can revert the forecaster back to those searches

Motivation:
Weather can either make or break someone's day. By giving one some predictability of the atmosphere, they can plan their days accordly to avoid obligations falling through or to cancel events that would be negatively impacted by the climate. A forecast of the current day as well as the coming week is a great way of accomplishing this.


Development:
To begin I made a skeletal html layout of exactly where I wanted the user input and content fields to be filled with weather data. Next I went to work testing how user imputes would be sent to local storage. I did this by assigning the input a key number one more then the length of the entries in local storage then setting their value to the user input itself then populating the html through DOM the user input as a button. I wrote a second function that would populate the search history field everytime the page was refreshed by using all the stored keys containing the user inputs. 
<img src = "https://github.com/pwg26/GetToKnowTheWeather/blob/master/images/ajax.png">

Next I used 2 ajax calls on 2 different openweather API’s- the first(a current weather forecast) to populate current weather content via DOM  the to pull required  latitude and longitude data from to be used for a 5 day open weather forecast. The data from the 5 day forecast was used to populate the corresponding content fields. 
<img src = "https://github.com/pwg26/GetToKnowTheWeather/blob/master/images/localstor.png">

Next I appended my two functions which generated the past search history buttons to have a click event which used the user input data to change to plug into the ajaxs to to change the forecast location. Lastly I styled the page with bootstrap and my original css.
<img src = "https://github.com/pwg26/GetToKnowTheWeather/blob/master/images/site.png">

Usage:
When the user opens the page it will be set to Denver Colorado. It will have the temperature, humidity, windspeed, uv index, and an icon displayed of the weather. When the user types in the city name and country or or state name separated by a comma, that city’s weather information will be displayed. The users searches will be saved so that they will populate under the search bar as a button so that if clicked it will display with weather information of that previous search city. 
