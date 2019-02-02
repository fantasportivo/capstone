<b>Introduction/Business Problem</b>

A home delivery company would like to start a marketing project to promote its services near to Toronto. First of all, firm decides to identify every districts of the city and to check for each of them the main restaurant in the area. The goal of this analysis is understanding where the advertising campaign have to take place. Than,  firm will try to group restaurants by proximity because different marketing strategies will be tested to identify the best way according to behavior of the citizens of the neighborhood.

The main subject interested in the analysis is certainly the company that has entrusted this project to a data scientist. A proper evaluation, moreover, will allow restaurateurs to take advantage of an additional home delivery service and data about customer preferences.

<b>Dataset</b>

In this analysis are used data relating to the different districts near to Toronto, after an activity of web scraping from a public wikipedia page. Starting from this database, we can identify restaurants where the advertising campaign will be taken and the subsequent clustering.
After identifying the corresponding latitude and longitude for each neighborhood, we proceed to search restaurant's data on foursquare site, using developer section.
The data obtained are filtered  in order to make clearer name of restaurant and its category, in addition to the respective coordinates of geolocation. The final result is a data merger that allow us to show on a map all restaurants divided, by colours, in 5 clusters.

<b>Methodology</b>

First of all, we import library useful to our analysis, such as pandas, numpy, random, request, matplotlib and more over(detailed in our report step by step). Pandas is early used to build a dataframe of neighborhoods and their latitude and longitude. In particular we used classic method of reading csv and transforming it into a dataframe (103 columns, 5 rows).
Next step is to discover what restaurants are near to our geolocations. In order to do that, we used foursquare site. In particular through an api we can extract venues and their characteristics. Data are extracted in a json file that has to be converted in a dataframe using jnormalize. Now we can filtered dataframe because a clear structure allow us to do a correct analysis.
Then, after loading folium library, we can show in a very simple, but detailed, map every neighborhood and their restaurants. This phase is important to do a first evaluation about our marketing strategy. In fact, we can observe where are concentrated more restaurants and in general their disposition.


