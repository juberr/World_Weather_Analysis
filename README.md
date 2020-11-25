# World Weather Analysis

The purpose of this repository is threefold:

 * Weather Database:

    * Creates a random list of 2000 longitudes and latitudes and uses the citipy library to identify the closest city to each.

    * Using the cities found with citipy, we obtain the current weather for each city using the OpenWeather API

    * Converts the data obtained from the previous two steps into a pandas dataframe, and exports it as a CSV

* Vacation Search:

    * Takes user input to filter the Weather Database dataframe based on their temperature tolerances.

    * Uses the user filtered dataframe to find hotels in each city using the Google Maps API, and appends that data to the dataframe.

    * Plots the hotel and weather data from the filtered dataframe onto a live Google Maps figure

* Vacation Itinerary:

    * Plots a trip with 4 stops in the same country in the Google Maps API using the filtered dataframe created in the Vacation Search deliverable