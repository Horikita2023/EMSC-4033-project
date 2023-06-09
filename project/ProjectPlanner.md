# The USGS earthquake data apply to Australia

## Executive summary

The USGS (United States Geological Survey) has the most detialed information of the earthquake in the world, but how can we apply this to our own countries? In this project, I plan to build a program when someone tape in parameters like time, maxmum magnititude, minimum magnititude, or the different states the map will show how earthquakes distrubutes in this area. This map will combine earthquake data with state map that users can acess the specific data in one state they ordered. This will help people get far away from the high risk places of earthquake, and alos can help local government make policies to reduce the loss from earthquake activities.

## Goals

There will be two goals in this project.

**First goal**: Select Australia earthquake data from USGS world earthquake data.

**Second goal**: apply Australia states map to earthquake data. Build a seclect system that allow people to choose their data in some specific conditions. Also try to give user ways to apply this data to their own situation.

## Background and Innovation  

This project aims to use the USGS earthquake data apply to Australia situation, which has several difficulties: how to get the earthquake data and apply it to map, how to select them by different states, and how to use this Url to get detial information of the earthquaqke.
The innovation of this project is to modify this map for most countries that people can use this for their own countries. People can input their own coordinate and they will get the nearest earthquake's information, this will help them make prepration or waring them where has more earthquakes during this time. 
Many people has done this before in different ways and for different perpose, such as:
`eq-mapper`: A Python script that fetches earthquake data from the USGS API and plots the earthquakes on a map using the Folium library.
`earthquake-mapper`: A web application that retrieves earthquake data from the USGS API and visualizes it on an interactive map using Leaflet.js and Python Flask.
`earthquake-data-mapping`: A Python script that fetches earthquake data from the USGS API and generates an interactive map using the Bokeh library.
so what I want to do is to make a more specific one that suitable for some countries and add some parameters inside.

## Resources & Timeline

The resources what I want to use is: 

USGS earthquake data base:'https://earthquake.usgs.gov/fdsnws/event/1/query'

The coordinate of state: 'https://www.ga.gov.au/'

Time line:

March: create plan, find the resource

Early April: create basic code on calculate earthquakes, plotting on the map

Later April: create input system, which users can sort by different parameters

May: test code, debug

## Test

This is the test plan for this project:

For the `obtain_earthquake_data` function:

Test the function by passing different combinations of parameters, such as varying start and end dates, different minimum magnitudes, and different geographical coordinates.
Check if the function returns a valid response from the earthquake data API.
Verify if the returned data contains the expected fields and format.

For the `map_plotting` part:

Test the map creation by checking if the plot is generated successfully using `plt.figure()` or `plt.subplots()`.
Test the addition of earthquake data points by providing test earthquake data and verifying if the points are correctly plotted on the map using plt.scatter() or similar functions.
Check if the map is displayed or saved correctly using `plt.show()` or `plt.savefig()`.

For the `coordinate` functions:

Test the latitude and longitude one by one to find out if the input is correct to work.
