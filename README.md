# Project 2 Cassandra
This is the second project for the Udacity data engineering nanodegree.

In this project we aim to process files into an Apache Cassandra database for Sparkify a music streaming 
service.


The jupyter notebook **Project_1B.ipynb** contains all the code needed to run this ETL.

The Part I section of the notebook relates to pre-processing the files. You will import the needed python 
packages and pre-process the files. We process all the csv files in the **/event_data** folder into one 
**event_datafile_new.csv** file which we will use in the next section.

In the Part II section, we load the **event_datafile_new.csv** into the different tables and 
then query the tables to see if they produce the required answers.

The creation and loading of the tables is based on optimizing read speeds. It is important to choose the 
right Primary Keys and Clustering Keys. The reasons for this are explained before each create table 
sql statement.

## Setup

This code will run on Python 3.9x. You will need to import below python packages :
1. cassandra-driver 
2. jupyter 
3. Pandas
4. Numpy
5. glob
6. json
7. csv

The rest of the packages imported in Part I first cell should be available by default in Python 3.9x
