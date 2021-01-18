# Creating webmaps using Python & Folium
Web maps typically represent locations and features from geographic data formats such as geoJSON and KML. Every location in a geographic data file can be considered to have geometry (such as points, lines, polygons) as well as additional properties. Web maps typically understand locations as a series of coordinates. For example, 28.7041, 77.1025 would represent the exact coordinates of New Delhi.

This project involves -

Reading data from a csv file using Pandas.
Creating a OpenStreet Base Map using Folium.
Adding Pointer Marker Feature to map.
Adding Multiple markers and Popup windows to map.
Color based pointer and styling them.
Using GeoJson data added a Polygon layer.
Adding a Layer Control Panel to the map.

We have used the following libraries of Python:
1. Folium - Folium is a Python library used for visualizing geospatial data. It is easy to use and yet a powerful library. Folium is a Python wrapper for Leaflet.js which is a leading open-source JavaScript library for plotting interactive maps. 
2. Pandas is another Python library that we will use. It’s a very popular library amongst scientists and mathematicians to manipulate and analyze data.

Folium gives a folium.Marker() class for plotting markers on a map. Just pass the latitude and longitude of the location, mention the popup and tooltip and add it to the map.
Folium also gives the folium.Icon() class which can be used for creating custom icons for markers which we have used in our WebMaps.

We have a text file that contains details about the volcanoes like coordinates, location, & height from sea level.
We have also attached a JSON file that contains the data like Population, Coordinates, etc

We've used latitudes and longitudes to plot markers; here’s how we did it:

1. Create a base map
2. Create a feature group for each category i.e., fgv - for Volcanoes & fgp - for Population
3. Then we add them to the feature groups
4. Finally, add these feature groups and layer control to the map
