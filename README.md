# Project Description
The ipython notebook is an attempt to segment the different neighborhoods in Toronto and see where one can find the best place to go if you want to party. It may be interesting for a real estate developer, prospective club owner, a business person looking to better understand the cities neighborhoods, etc. This is done by scraping web data from wikipedia, to obtain the borough and neighborhoods corresponding to each postal code in Toronto. Geopy's geolocator feature is then used to match each postal code to a latitude and longitude that will later be used when visualizing the clustering results on a map provided by the folium API. The clustering is done by looking at the venues in each region, data which is obtained by calling the Foursquare API to access its massive dataset of locations, venues, user reviews, etc. The neighborhoods are then grouped and sorted according to the most common types of venues and clustered by using the [kmeans clustering algorithm](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html). Additional analysis shows where the night life and party hubs of the city are. 

# Requirements/Dependencies
- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/) for web scraping
- [requests](http://docs.python-requests.org/en/master/user/install/#install) for web scraping
- [geopy](https://pypi.org/project/geopy/) for accessing location data
- [tqdm](https://pypi.org/project/tqdm/) for displaying progress bars
- [folium](https://github.com/python-visualization/folium) for mapping data
- [sklearn](https://scikit-learn.org/stable/install.html) for running the kmeans algorithm
