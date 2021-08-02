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
I registered for an OpenweatherMap API Key.  The API key is not included this this repository.  I requested and retrieved data from the website and parsed the data using JavaScript Object Notation (JSON).  I retrieved weather data for over 500 cities, parsed it using JSON and converted the dictionary array to a DataFrame.  After creating the DataFrame, I reordered the columns so the table would be easier to read.  As a final step, I exported the DataFrame to a CSV file.
## Lesson 3
I dedicated time to creating a community outreach website for middle school STEM students with the approval of my supervisor.  I used the weather data collected for the 500+ cities from around the world to create scatter plots.  The first plot was City Latitudes versus Maximum Temperature.  For my dataset, maximum temperatures above 90 degrees F occurred between latitudes 18 degrees N to 60 degrees N.  The City Latitude versus Humidity plot showed that there are a lot of cities with humidity percentages greater than 60%.  Wow.  I live in a high desert climate; I die when the humidity reaches 15% or greater.  Nothing out of the ordinary was noted on the City Latitude versus Cloudiness plot.  The final plot, City Latitude versus Wind Speed showed the highest concentration of wind speeds between 0 to 10 miles per hour occurred around latitudes 22 degrees N to 70 degrees N. 
## Lesson 4
I created scatter plots for each weather parameter on the Northern and Southern Hemispheres.  I added regression line equations and correlation coefficients to each plot to help the STEM students determine correlations between weather data and latitudes.  The correlation between the latitude and maximum temperture is strong:  the temperatures become warmer as we approach the equator.  For humidity, the correlation is very low, which means that percent humidity is unpredictable due to changing weather pattern across the latitudes.  Once again, the correlation between the percent cloudiness and latitude is very low; cloudiness is unpredictable due to changing weather patterns.  Like the previous two plots, the correlation between the latitude and wind speed is very low.  Latitude has very little impact on determining wind speed.  
## Lesson 5
In this lesson, I had a lot of trouble getting my heatmaps to load despite installing the gmaps dependency.  I created several heatmaps to help vacationers choose their ideal vacation spot. 
