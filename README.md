# sqlalchemy-challenge

# Part 1: Analyze and Explore the Climate Data

Used the provided files (climate_starter.ipynb and hawaii.sqlite) to complete your climate analysis and data exploration

Use the SQLAlchemy create_engine() function to connect to your SQLite database.

Use the SQLAlchemy automap_base() function to reflect your tables into classes, and then save references to the classes named station and measurement.

Link Python to the database by creating a SQLAlchemy session.

# Precipitation Analysis

Create a query that finds the most recent date in the dataset 

Create a query that collects only the date and precipitation for the last year of data without passing the date as a variable

Save the query results to a Pandas DataFrame to create date and precipitation columns

Sort the DataFrame by date

Plot the results by using the DataFrame plot method with date as the x and precipitation as the y variables 

Use Pandas to print the summary statistics for the precipitation data

# Station Analysis

Design a query that correctly finds the number of stations in the dataset

Design a query that correctly lists the stations and observation counts in descending order and finds the most active station

Design a query that correctly finds the min, max, and average temperatures for the most active station

Design a query to get the previous 12 months of temperature observation (TOBS) data that filters by the station that has the greatest number of observations

Save the query results to a Pandas DataFrame 

Correctly plot a histogram with bins=12 for the last year of data using tobs as the column to count.

# Part 2: Design Your Climate App

/
Start at the homepage.
List all the available routes.

/api/v1.0/precipitation
Convert the query results from your precipitation analysis (i.e. retrieve only the last 12 months of data) to a dictionary using date as the key and prcp as the value.
Return the JSON representation of your dictionary.

/api/v1.0/stations
Return a JSON list of stations from the dataset.

/api/v1.0/tobs
Query the dates and temperature observations of the most-active station for the previous year of data.
Return a JSON list of temperature observations for the previous year.

/api/v1.0/<start> and /api/v1.0/<start>/<end>
Return a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a specified start or start-end range.
For a specified start, calculate TMIN, TAVG, and TMAX for all the dates greater than or equal to the start date.
For a specified start date and end date, calculate TMIN, TAVG, and TMAX for the dates from the start date to the end date, inclusive.

