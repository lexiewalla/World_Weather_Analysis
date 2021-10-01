# World_Weather_Analysis

### Overview
The purpose of this project was to use our new knowledge on APIs and create a vacation search application. We obtained the API keys for openweathermaps and googlemaps and were able to utilize these keys to obtain weather data from openweather and map data from google.

I used the openweather API to pull weather data from over 500+ cities. From there we created a prompt for users to put in their temperature preferences for minimum and maximum temperatures a city has. The temperatures the user puts in will pull from the weather data we retrieved from the 500 hundred cities. I created a dataframe with all the cities and weather information and imported it into a csv file named Weather Databse.

The weather database csv file was imported into another dataframe and created a column named "Hotel". We were able to use the nearby google search to retrieve the JSON data to find hotels within the vicinity of the cities that have the preferred weather the user chose. The hotels in those cities were imported into the new dataframe. I took the new dataframe and imported the hotel information and weather information into a new CSV file named Vacation Database.

<img width="915" alt="FigDel1" src="https://user-images.githubusercontent.com/45208773/135661339-84eac5f2-6862-4aa3-b810-79d956c1e18f.PNG">

From there, these dateaframes creates a map with markers to see where each city is. We were able to create this map with the markers using gmaps. This is what will appear in the application to the user after choosing the temps preferences.

<img width="871" alt="WeatherPy_travel_map_markers" src="https://user-images.githubusercontent.com/45208773/135661125-c66da8ad-735a-4fcc-b6ce-d17cc76d1b24.PNG">
 

After exploring the map, and acting like a user, I chose 4 cities in Europe. With the preferred weather and the hotel info we created made another map using gmaps that marks just those four specific cities and hotels to stay in. When you click on the markers, and information box appears showing the city, country, max temps, and current weather descriptions. 

<img width="863" alt="WeatherPy_vacation_map" src="https://user-images.githubusercontent.com/45208773/135661093-0dfe0979-1fa3-43d3-b756-f7bc37d72028.PNG">


The app is supposed to create a "travel itinerary" for the user. It can create walking directions, biking or driving directions. For this trip, as the user, I chose driving directions. I then created another map using gmaps directions layer, adding in starting and ending points and 3 stops in the middle. The app will print out a map with directions starting at the starting point, hitting all three stops in between and ending back at the starting point!

<img width="666" alt="WeatherPy_travel_map" src="https://user-images.githubusercontent.com/45208773/135661960-74d33426-b0dc-4559-a060-d4bad85073b3.PNG">
