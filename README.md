# GDELT Engineering
The repository contains the code for Medical Protest Event Prediction on GDELT data.<br/>

The Project aim is to extract the data for medical unrest event, transform the data and load it to database. Then to apply datamodels to the generated dataset to classify the events as protest and non-protest causing events.

The directory Abhinav Sharma - sc21as consists of the following items.
1. Raw data file collection system : It is a data collection system developed for local machine to collect the medical protest event data from GDELT
2. Three Jupyter notebooks
    1. Data Exploration and HMM : Contains the code for data exploration on the original data extracted from Google BigQuery of GDELT Event 2.0 Database
    2. Feature Generation : Performs feature engineering on the dataset and produces a new dataset to be used to make prediction
    3. ML Predictions : Test the generated dataset on the ML models. Used for testing of the generated data
3. Dataset : Contains the datasets generated after applying feature engineering. Consists of two files 
    1. Balanced_Data_All.zip : Consists of CSV file containing all the data extracted from BigQuery along with the new feature "Target". It is compressed as the size is large. 
The direcotry Data collection system consists of the system to collect the data from GDELT and combine it to one CSV file and later upload it to a MongoDB database.<br/>
The collection system collects the event table data uploaded by GDELT in the Master data file. https://www.gdeltproject.org/. The subdirectories are used to store the downloaded data temporarily before it is uncompressed and combined into one csv.
