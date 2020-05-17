# Udacity-Data_Modeling-with-Apache_Cassandra
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.  They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions, and wish to bring you on the project. Your role is to create a database for this analysis. You'll be able to test your database by running queries given to you by the analytics team from Sparkify to create the results.

# Project Overview
In this project, you'll apply what you've learned on data modeling with Apache Cassandra and complete an ETL pipeline using Python. To complete the project, you will need to model your data by creating tables in Apache Cassandra to run queries. You are provided with part of the ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.

We have provided you with a project template that takes care of all the imports and provides a structure for ETL pipeline you'd need to process this data.

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
