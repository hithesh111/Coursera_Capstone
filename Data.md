<h1>New City Neighborhood Project</h1>

<h2>Data used</h2>

<h3>Wikipedia page</h3>
Scrapped the <a href = 'https://en.wikipedia.org/wiki/List_of_neighbourhoods_in_Bangalore'> Wikipedia Page </a> about Zones and Neighborhoods in Bangalore. It has zone-wise tables with rows being neighborhoods in the zone and the description of the neighborhood. The description, however is not relevant to our project and the column is dropped.

<h3>Latitudes and Longitudes (Google)</h3>
Since there were only ~60 neighborhoods, googling for coordinates of these was feasible. I have entered latitudes and longitudes of these neighborhoods manually and uploaded the data <a href = 'https://github.com/hithesh111/Coursera_Capstone/blob/master/neighborhood_lat_long.csv'> here. </a>

<h3>FourSquare Location Data</h3>
And most importantly,<a href = 'https://foursquare.com/'>FourSquare</a> data was used to fetch location-based results using their <a href = 'https://foursquare.com/developers'>Developer Portal</a>.<br>
The API was used to get information about various venues and their details (like name, category, latitude, longitude) within some radius around points on the map. The 4 details mentioned above were most important to create onehot encodings of frequency of venues in neighborhoods which was then used to cluster the neighborhoods.<br><br>
The user's top few priorities are also represented as a onehot vector and then the cluster prediction is done on this vector.
