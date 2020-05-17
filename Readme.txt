Sparkify Cassandra ETL :  1B - Project submission for the Data Engineering Nanodegree.

This project consists of putting into practice the following concepts:

1. Data modeling with Cassandra
2. ETL pipeline using Python

Project Summary

Data pre-processing, ETL pipeline, and data modeling. The data are stored as a collection of csv files partitioned by date. 
The ETL pipeline and data modeling are written in a single jupyter notebook, Project_1B_Project_Template.ipynb.

ETL copies data from the date-partitioned csv files to a single csv file event_datafile_new.csv which is used to populate the denormalized Cassandra tables optimised for the 3 queries above. 
The 3 tables in the model are named after the song play query they are created to solve:

1. session_songs includes artist, song title and song length information for a given sessionId and itemInSessionId.
2. event_log includes artist, song and user for a given userId and sessionId.
3. song_users includes user names for a given song.