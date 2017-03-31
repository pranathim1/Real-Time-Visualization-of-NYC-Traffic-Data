# Real-Time-Visualization-of-NYC-Traffic-Data
In this project, we chose to use the <a href="http://207.251.86.229/nyc-links-cams/LinkSpeedQuery.txt">real-time data stream</a> of New York City traffic data which is collected from the sensors located on major arterials and highways within the city limits.
The traffic data updates several times per minute, but the updating frequency varies in a
day. Fields in the dataset includes the “Transcom Link ID”, “average speed” a vehicles traveled
between end points on the link in the most recent interval, “time” the average vehicle took to
traverse the link, “latitude” and “longitude” of the sensor links in Google compatible polyline
form, and more.

We used python web scraping to collect the data stream and used Apache Spark for data
stream processing. We then performed analysis on the streaming data in order to understand
how the average speed and time taken for travel is varying across different transcom links and
the four boroughs. We next visualized our findings with plotly, which refreshed every 6 seconds
to show the timely changes from the streaming data.
