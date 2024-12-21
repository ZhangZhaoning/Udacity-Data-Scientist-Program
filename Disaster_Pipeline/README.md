# Disaster Response Pipeline Project

## Project Overview

This project is part of the Udacity Data Science Nanodegree program and focuses on building a machine learning pipeline to categorize disaster-related messages. The goal is to assist disaster response agencies in directing messages to the appropriate departments quickly and effectively.

## The project includes:
	•	An ETL pipeline for cleaning and preparing the data.
	•	A machine learning pipeline for training a multi-output classifier to predict multiple categories for each message.
	•	A Flask web application where users can input a disaster message and get classification results, along with visualizations of the data.

 File Structure:
- app
| - template
| |- master.html  # main page of web app
| |- go.html  # classification result page of web app
|- run.py  # Flask file that runs app

- data
|- disaster_categories.csv  # data to process 
|- disaster_messages.csv  # data to process
|- process_data.py
|- InsertDatabaseName.db   # database to save clean data to

- models
|- train_classifier.py
|- classifier.pkl  # saved model 

- README.md

## Key Features
	1.	ETL Pipeline:
	•	Extracts data from raw datasets (messages.csv and categories.csv).
	•	Cleans and transforms the data.
	•	Stores the processed data in an SQLite database for easy access.
	2.	Machine Learning Pipeline:
	•	Tokenizes and processes text messages.
	•	Trains a multi-output classifier to predict 36 disaster-related categories.
	•	Tunes hyperparameters using GridSearchCV for optimal performance.
	3.	Flask Web Application:
	•	Provides an interface for users to input messages and view classification results.
	•	Displays data visualizations for better insights into disaster messaging patterns.

 ![image](https://github.com/user-attachments/assets/44ad8fba-73af-47d5-855c-e8cfc1268e1a)


