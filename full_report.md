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
Now, one of the most  important phases of our analysis is k-means clustering. This method allow us to segment restaurants in group useful in the next step of the marketing strategy. In particular we defined 5 clusters and we showed them into a map with different colours. Clustering is necessary beacuse our scope is to starting an advertising campaign and we want to understand how we can test different strategy in every group with similar characteristics. This simplify also next analysis of customers behaviour in every single neighborhood.

<b>Results</b>

Results of our analysis are based on the final process of clustering. In fact we can support firm that has commissioned this project through the definition of 5 peer groups where it can develop its marketing strategy. The importance of this analysis is connected to the ability of simplify decisions that firm have to take. In fact is too expensive starting a campaign in every restaurants and is less efficient applying the same strategy to every neighborhoods. Moreover this analysis is a base for a next evaluation about customers' behaviours. 

<b>Discussion section</b>

In order to being useful, this analysis have to be supported by a successive evaluation. In particular, we can apply 2 different strategies: first of all, firm can test for each group a lot of advertising campain and than select for every single group the best one; second, the firm can develop a trend analysis in every group, also using foursquare site in order to understand if there are trends that can justify a particular marketing strategy.
In order to being useful, this analysis have to be supported by a successive evaluation. In particular, we can apply to different strategies: first of all, firm can test for each group a lot of advertising campain and than select for every single group the best one; second, the firm can develop a trend analysis in every group, also using foursquare site in order to understand if there are trends that can justify a particular marketing strategy.
Moreover, we can evaluate if there are already delivery services in theese areas. In fact if we want to start with a new business is not enough to develop our strategy but is important to analyze how our competitors work and how they can react to our presence.

<b>Conclusion</b>

As every analysis, results are just the beginning for other evaluations and analysis. Power of results are simply an opportunity to discover new aspects and develop project in different areas of study. Ability of a data scientist is to observe reality and to image results of his analysis as a starting point for a more complex structure. This were the initial goals of this analysis and i hope to have reached them.
