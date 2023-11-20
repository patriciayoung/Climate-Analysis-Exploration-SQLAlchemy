# sqlalchemy-challenge

Version of SQLAlchemy I am running is 1.4.3
This high the needed to know when running the Jupyter notebook.

SurfsUp directory contains climate.ipynb Jupyter Notebook, app.py Python scrip, and a Resources folder that contains the hawaii.sqlite database, hawaii_measurements.csv, and hawaii_stations.csv.



Part 1: Analyze and Explore the Climate Data
Climate Analysis and data exploration was done on the hawaii_sqlite database. The Jupyter notebook was created to preform Precipitation and Station Analyses. The app.py python script was created to design climate app with Flask API with JSON lists of climate information.


Precipitation Analysis: ORM queries were done to obtain date and prcp data for previous 12 months. Pandas DF was created using queried data. Results were plotted using Matplotlib. And summary stats were obtained for prep for previous 12 months.

Station Analysis: All stations and their number counts were listed in desc order. Min, avg, and max temps were queried for most active station (by id). Last 12 months of temp observation data was queried. Results were plotted using Matplotlib. 



Part 2: Design Your Climate App

A Climate API was created using Flask. The following 5 routes are available routes created using Flask:

1. / (Homepage)
Start at the homepage.

List all the available routes.

2. /api/v1.0/precipitation (Precipitation)
Convert the query results from your precipitation analysis (i.e. retrieve only the last 12 months of data) to a dictionary using date as the key and prcp as the value.

Return the JSON representation of your dictionary.

3. /api/v1.0/stations (Stations)
Return a JSON list of stations from the dataset.

4. /api/v1.0/tobs (TOBS)
Query the dates and temperature observations of the most-active station for the previous year of data.

Return a JSON list of temperature observations for the previous year.

5. /api/v1.0/<start> and /api/v1.0/<start>/<end> (minimum, average, and maximum temperature for a specified start or start-end range)
Return a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a specified start or start-end range.

For a specified start, calculate TMIN, TAVG, and TMAX for all the dates greater than or equal to the start date.

For a specified start date and end date, calculate TMIN, TAVG, and TMAX for the dates from the start date to the end date, inclusive.


