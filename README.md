# World_Weather_Analysis

# Project Overview
The PlanMyTrip app is currently being tested in a beta setting with the objective of enhancing user interface and functionalities through the following steps:

    1. Retrieving weather data including the weather description for over 150 cities across the world,
    2. Create a customer travel destinations map,
    3. Create a travel itinerary map.

## Resources
- Data Source: [citipy](https://github.com/wingchen/citipy), [jupyter-gmaps](https://jupyter-gmaps.readthedocs.io/en/latest/), [OpenWeatherMap API](https://openweathermap.org/current), [Google Maps and Places API](https://developers.google.com/places/web-service/search), [Google Maps Directions API](https://developers.google.com/maps/documentation/directions/overview)

- Software: Python 3.7.7, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Retrieve weather data
Through the NumPy dependency we have generated 2,000 sets of coordinates (latitude and longitude). Through these coordinates Python's cityp module is then used to identify the nearest city for each coordinate combination. The weatherdata is retrieved for all identified cities through a request to the OpenWeatherMap API. In this case 706 cities were identified.

![WeatherPy_weather_data](https://user-images.githubusercontent.com/88256967/133952513-1708e894-5203-4908-9921-02c8164f98e4.PNG)

## Create a customer travel destinations map

The app required customer to input their minimum and maximum temperatures for their trip.

![Customer Input](https://user-images.githubusercontent.com/88256967/133952498-7fd0746a-c611-4158-928d-aa53735146b5.PNG)


Once this was completed the app uses the inputs to filter the cities that fit the criterea which in this case was only 193.

![WeatherPy_vacation_list](https://user-images.githubusercontent.com/88256967/133952579-0a4bfaf7-643f-43e9-80ee-e826f4b0bc03.PNG)

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/88256967/133952593-e01a1d47-2a50-483d-979a-5cdc3701eb4a.PNG)

## Create a travel itinerary map

After reviewing the 193 cities that met the criteria for the weather requested by the customer we suggested 4 cities in Europe that can be a great travel destination.

![WeatherPy_travel_list](https://user-images.githubusercontent.com/88256967/133952702-ad8a1f2d-30b0-47ab-ae02-a94724c07c09.PNG)

Below is the route:
  1. Kirakira, PT (Begin)
  2. Santa Eulalia Del Rio, ES
  3. Lannion, FR
  4. Pavullo Nel Frignano, IT
  5. Kirakira, PT (End)

![WeatherPy_travel_map](https://user-images.githubusercontent.com/88256967/133952713-2baf2227-40dd-4d6e-a133-15132f460df5.PNG)

Below maps will show map markers with info box.

![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/88256967/133952718-8f05a728-d5cd-4dd9-9a5e-695307a9d760.PNG)

![WeatherPy_travel_map_markers2](https://user-images.githubusercontent.com/88256967/133952722-71261ddb-521c-4635-8c89-335d7d7dc41a.PNG)


