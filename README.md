# Sparkify-Cassandra-ETL
Data Modeling with Cassandra on song play analysis.  

### Problem definition
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.  

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions, and wish to bring you on the project.  

We have provided you with a project template that takes care of all the imports and provides a structure for ETL pipeline you'd need to process this data.  

### Files  
#### CassandraProject.ipynb
- Load original event csv data files into a new event_datafile_new.csv file for non-empty artist fields.
- Create cassandra a keyspace named "sparkify" for the tables
- Create Cassandra tables answer these 3 queries:
	1. Give the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
	2. Give only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182  
	3. Give every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own
- And display the output.  

#### event_data/
This directory contains csv files which needs to be processed and loaded into database.