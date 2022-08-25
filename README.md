# GDELT
The repository contains the code for Medical Protest Event Prediction on GDELT data.<br/>

The Project aim is to extract the data for medical unrest event, transform the data and load it to database. Then to apply datamodels to the generated dataset to classify the events as protest and non-protest causing events.

The project division is done into two parts.

Abhinav Sharma - sc21as : Data extraction , transformation, load and feature engineering. Generating the datasets and creating a real-time dashboard using GDELT API 
Lohavani Sevveral - sc21ls : 

#### The directory Abhinav Sharma - sc21as consists of the following items.
1. Raw data file collection system : It is a data collection system developed for local machine to collect the medical protest event data from GDELT
2. Jupyter notebooks
    1. Data Exploration and HMM : Contains the code for data exploration on the original data extracted from Google BigQuery of GDELT Event 2.0 Database
    2. Feature Generation : Performs feature engineering on the dataset and produces a new dataset to be used to make prediction
    3. ML Predictions : Test the generated dataset on the ML models. Used for testing of the generated data
    4. MongoDB : Code to push the generated data to MongoDB database. Creating two collections for two dataset files
3. Dataset : Contains the datasets generated after applying feature engineering. Consists of two files 
    1. Balanced_Data_All.zip : Consists of CSV file containing all the data extracted from BigQuery along with the new feature "Target". It is compressed as the size is large. 
    2. Balanced_Data_No_Protest_Code_Significant : Consists of the dataset file in CSV format having the cleaned data with only significant features
4. MongoDB Dump.zip : Consists of the dump of the GDELT database in MongoDB. Consists of BSON file
5. dashboard.html : Consists the dashboard for medical protest data using the GDELT 2.0 DOC API


