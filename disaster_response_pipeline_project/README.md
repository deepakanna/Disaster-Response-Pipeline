# Disaster Response Pipeline Project
## Project Description:
This project aims to analyse the disaster data from Figure Eight and to build a model that classifies the messages into specific categories during disaster. The dataset contains 30000 messages obtained from an earthquake in Haiti in 2010, an earthquake in Chile in 2010, floods in Pakistan in 2010, superstorm Sandy in the U.S.A. in 2012, and news articles spanning a large number of years and 100s of different disasters. The specific categories are 36 namely medical_help,child_alone,death, missing_people, floods etc. This helps the emergency organizations to help the needy during a disaster. This project involves building an ETL pipeline that facilitates Extraction, Transformation and loading the disaster data, followed by a Machine Learning pipeline where a pipeline is designed using CountVectorizer, TfidfTransformer and a Multioutputclassifier is used. A Web app is developed that gives the classification output for an input message. 

## Project Sections:
1. ETL Pipeline:
    - Pipeline to Extract, Transform and Load Data
    - Save it in SQLite Database
3. ML Pipeline:
    - Load data from SQLite
    - Text Data processing 
    - ML pipeline 
    - Using GridSearchCV to determine the final model for classification
5. Web Development:
    - Design using HTML
    - Build Web application using Flask

## Requirements:
This project requires Python 3 with pandas, numpy, sklearn, plotly, nltk, sqlalchemy, pickle installed.

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/


