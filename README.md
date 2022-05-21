# Project: Data Modeling with Postgres

## Introduction

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to.

The main purpose is to create a Postgres database with tables designed to optimize queries on Song Play Analysis.

## Project Description

In this project, you'll apply what you've learned on data modeling with Postgres and build an ETL pipeline using Python. To complete the project, you will need to define fact and dimension tables for a star schema for a particular analytic focus, and write an ETL pipeline that transfers data from files in two local directories into these tables in Postgres using Python and SQL.

## Build schema for Song Play Analysis
**Fact Table**

*songplays* records in log data associated with song plays
    
**Dimension Tables**

*users* in the app

*songs* in music database

*artists* in music database

*time* - timestamps of records in songplays broken down into specific units

## Project Design

The project includes the following 6 files:

*test.ipynb* - displays the first few rows of each table to let you check your database.

*create_tables.py* - drops and creates your tables. You run this file to reset your tables before each time you run your ETL scripts.

*etl.ipynb* - reads and processes a single file from *song_data* and *log_data* and loads the data into your tables. This notebook contains detailed instructions on the ETL process for each of the tables.

*etl.py* - reads and processes files from *song_data* and *log_data* and loads them into your tables. You can fill this out based on your work in the ETL notebook.

*sql_queries.py* - contains all your sql queries, and is imported into the last three files above.

*README.md* - provides project description.

## Project Steps

*Step 1*:

**Create Tables**:

* Write CREATE statements in *sql_queries.py* to create each table.
    
* Write DROP statements in *sql_queries.py* to drop each table if it exists.
    
* Run *create_tables.py* to create your database and tables.
    
* Run *test.ipynb* to confirm the creation of your tables with the correct columns.

*Step 2*:

**Build ETL Processes**: 

* Use *etl.ipynb* notebook to develop ETL processes for each table. 

* At the end of each table section, or at the end of the notebook, run *test.ipynb* to confirm that records were successfully inserted into each table. 

* Rerun *create_tables.py* to reset your tables before each time you run this notebook.

*Step 3*:

**Build ETL Pipeline**:

* Use what you've completed in *etl.ipynb* to complete *etl.py*, where you'll process the entire datasets. 

* Run *create_tables.py* before run *etl.py* to reset your tables. 

* Run *test.ipynb* to confirm your records were successfully inserted into each table.


