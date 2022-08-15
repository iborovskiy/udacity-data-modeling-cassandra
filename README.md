### Date created
2022-08-15


### Project Title
Udacity course project: Data Modeling with Apache Cassandra


### General Description
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app.
The analysis team is particularly interested in understanding what songs users are listening to.

The goal of this project is to create an Apache Cassandra database with tables designed to answer the questions (queries) on song play analysis.
In this project, the following data modeling tasks were completed:
1. Modeling NoSQL database to answer the queries outlined by the analysis team
2. Defining logic to create and delete Apache Cassandra keyspace tables
3. Building ETL pipeline that collects data from the original data files into the target csv file and inserts that data into DB tables.


### Details of database design and ETL pipeline
For this project, we must answer following three questions:
1. **Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4**
2. **Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182**
3. **Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'**

We model and create three db tables to answer these questions:
1. session_song_library
2. session_library
3. song_history_library

**ETL pipeline** performs the following functions:
1. Reads data from csv-log files
2. Collect this data into the single composite csv file: **event_datafile_new.csv**
![Example of the song play events log file](/images/image_event_datafile_new.jpg "Example of the song play events log file")


### Instructions for running the Python scripts
All the necessary scripts for running ETL pipeline and creating/deleting DB tables are contained in Jupyter notebook:
- **Project_1B_Sparkify_iborovskiy.ipynb**
You must run corresponding sections of this notebook to carry out different tasks of workflow.


### Credits
**This entire project is based on learning materials from Udacity:**
https://learn.udacity.com/
