# World_Weather_Analysis
## Introduction
In this module, I will learn how to gather website data using APIs.  I work for a company called PLANMYTRIP, which specializes in Internet-related services for the hotel and lodging industries.  Jack is head of analysis for the user interface team.  He wants to know how the company can provide real-time suggestions for our client's "ideal" hotels.  In Jack's perspective, "ideal" hotels are:  
1.  within a given range of latitude and longitude, and
2.  provide the right weather for the client.  

A project outline is as follows:  
  * Task: Collect and analyze weather data across cities worldwide.
  * Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
  * Method: Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail       collecting, analyzing, and visualizing the data.
The data analysis will be split into three main parts, or stages.

  1.  Collect the Data
      * Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
      * Use the citipy module to list the nearest city to the latitudes and longitudes.
      * Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
      * Parse the JSON data from the API request.
      * Collect the following data from the JSON file and add it to a DataFrame:
          a.  City, country, and date
          b.  Latitude and longitude
          c.  Maximum temperature
          d.  Humidity
          e.  Cloudiness
          f.  Wind speed
         
  2. Exploratory Analysis with Visualization
     -  Create scatter plots of the weather data for the following comparisons:
        - Latitude versus temperature
        - Latitude versus humidity
        - Latitude versus cloudiness
        - Latitude versus wind speed
     -  Determine the correlations for the following weather data:
        - Latitude and temperature
        - Latitude and humidity
        - Latitude and cloudiness
        - Latitude and wind speed
        - 
     -  Create a series of heatmaps using the Google Maps and Places API that showcases the following:
        - Latitude and temperature
        - Latitude and humidity
        - Latitude and cloudiness
        - Latitude and wind speed
  3.  Visualize Travel Data
      Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these       steps:
      - Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
      - Create a heatmap for the new DataFrame.
      - Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
      - Store the name of the first hotel in the DataFrame.
      - Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.
## Lesson 1
In this lesson, I learned about four different random functions available through the random module.  Using Numpy and Random modules, I generated a random list of latitude and longitude coordinates using 1,500 as the size limit.  I used Python's citipy module with a "for" loop to generate a list of over 600 cities.
## Lesson 2
I registered for an OpenweatherMap API Key and saved it in a safe place.  I requested and retrieved data from the website and parsed the data using JavaScript Object Notation (JSON).  I retrieved weather data for over 500 cities, parsed it using JSON and converted the dictionary array to a DataFrame.  After creating the DataFrame, I reordered the columns so the table would be easier to read.  As a final step, I exported the DataFrame to a CSV file.
