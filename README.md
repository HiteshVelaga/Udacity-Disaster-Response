# Udacity-Disaster-Response

## Project Motivation<a name="motivation"></a>


In this project, I have used analyze disaster data from [Figure Eight](https://www.figure-eight.com) to build a model for an API that classifies disaster messages.

I have created an ETL pipeline that loads and cleans the data into a database to make it ready for modelling and analyzing

Then, an ML pipeline is incorporated that tokenizes the data and builds a supervised ML pipeline for classification

Finally, a web app using Flask is built to visualize the data and show the classification results.



## File Descriptions <a name="files"></a>

`data/process_data.py` runs the ETL pipeline. It takes as input on command line the csv file names and the destination database path. For instance, to run the file, navigate to the data folder and type the following: \
```python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db```

`models/train_classifier.py` runs the ML pipeline. It takes as input on command line the database path and the destination model pickle file. For instance, to run the file, navigate to the models folder and type the following: \
```python train_classifier.py ../data/DisasterResponse.db classifier.pkl``` 

`app/run.py` runs the Flask web app. To run it simply type `python run.py` in the app folder.
