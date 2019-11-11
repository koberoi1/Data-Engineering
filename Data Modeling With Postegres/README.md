# Data Modeling with Postegres



This is the first project submission for the Data Engineering Nanodegree. This project consists on putting into practice the following concepts:

1. Data modeling with Postgres
2. Database star schema 
3. ETL pipeline using Python


## Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app

 ***The aim is to create a Postgres Database Schema and ETL pipeline to optimize queries for song play analysis.***

## Project structure

### Files
1. data : JSON files
2. sql_queries.py :  contains all your sql queries
3. create_tables.py: drops and creates tables. Run this file everytme before running etl.py
4. test.ipynb:  prints the first few rows of each table 
5. etl.ipynb : ETL pipeline, exracts and
6. etl.py 
7. README.md 

### execute files in the below order each time 

```
$ python3 create_tables.py
```

```
$ python3 etl.py
```

## Created a STAR schema
* **Fact** Table: songplays: attributes referencing to the dimension tables.
* **Dimension** Tables: users, songs, artists and time table.


## ETL pipeline 
1. Created songs, artist dimension tables from extracting songs_data by selected columns.
2. Created users, time dimension tables from extracting log_data by selected columns.
3. Created the most important table fact table from the dimensison tables and log_data called songplays.



