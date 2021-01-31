# World_Weather_Analysis

## Project Overview

The purpose of the project was to build an app that allows the user to find possible vacation destinations based on the current weather conditions they desired, specifically temperature.  The app will also provide the user with a hotel in the possible destination cities, and then provide them with a mapped round trip between their chosen city and three others they could visit while on the trip

## Resources

Python 3.7.9, Jupyter Notebook, OpenWeatherMap.org Current Weather API, Google Places API, Google Maps Directions API, jupyter-gmaps,citipy

## Summary

The app randomly generates 2,000 sets of latitude and longitude, then using citipy finds the nearest city to each set of coordinates.  For coordinates not near any city (for example coordinates in a body of water) no city is chosen.

Using the OpenWeatherMap.org Current Weather API, the app finds the current weather conditions, including maximum daily temperature, for each city in the list.  The user is then prompted to enter their preferred hi and low temperatures for their possible destinations.  A map is then generated of the cities falling in that temperature range using jupyter-gmaps and hotel information provided from the Google Places API.  Each city on the map has a popup box that displays the current weather in that city as well as a possible hotel.

The app then has the capability to generate a mapped route for a round trip between four cities from the list, should the user desire to explore more cities around their chosen vacation destination.

