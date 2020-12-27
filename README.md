# Disaster Response Pipeline Project

Link to the Github Repository of this project: https://github.com/gunanksood/Disaster_Response_Pipeline

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/


### About this Project

I worked on this project as a part of Data Science Nanodegree, Code template and Dataset is provided by Udacity.

This project uses Python3 and a few Libraries listed below:

1. NumPy <br>
2. Pandas <br>
3. Matplotlib <br>
4. Json <br>
5. Plotly <br>
6. Nltk <br>
7. Flask <br>
8. Sklearn <br>
9. Sqlalchemy <br>
10. Sys <br>
11. Re <br>
12. Pickle <br>

### About Files

disaster_messages.csv, disaster_categories.csv contain sample messages (real messages that were sent during disaster events) and categories datasets in csv format provided by Udacity.

templates folder: This folder contains all of the files necessary to run and render the web app.

process_data.py: This file reads data from both CSV files: messages.csv (containing message data) and categories.csv (classes of messages) and creates an SQLite database containing a merged and Processed/Cleaned data which can be consumed by model.

train_classifier.py: This file reads processed data from Sqlite db as an input and uses the data to train and tune a ML model for categorization of messages. Creates a pickle file containing the trained model. Test evaluation metrics are also printed as part of the Model Evaluation process.



