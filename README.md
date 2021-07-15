# Udacity-DisasterResponse-Pipeline

This repository contains my udacity project on Disaster Response Pipline

# Motivation for this project
The motivation for doing this project was primarily an interest in undertaking a challenging project in an interesting area of research.

# Libraries Used
- numpy 
- pandas 
- nltk
- sys
- re
- sklearn 
- sqlalchemy
- pickle

# Project Description:
In this project, we will build a web app to classify messages that are sent during disasters, using machine learning. There are 36 pre-defined categories, and examples of these categories include  Medical Help, Search And Rescue, etc. By classifying these messages, we can allow these messages to be sent to the appropriate disaster relief agency. This project will involve the building of a basic ETL and Machine Learning pipeline to facilitate the task. This is also a multi-label classification task, since a message can belong to one or more categories. We will be working with a data set provided by Figure Eight containing real messages that were sent during disaster events.

Finally, this project contains a web app where you can input a message and get classification results.

![uss3](https://user-images.githubusercontent.com/72887048/125740623-2af6f107-26ae-4b53-bf9e-2508839583cb.png)



# File description:
1) app:
   - template
            master.html: main page of web app.
            go.html: classification result page of web app.
   - run.py: Flask file that runs app.

2) data:
   - data_messages.csv: messages data provided by figure8.
   - data_categories.csv: categories data provided by figure8.
   - DisasterResponse.db: Database to save clean data.
   - process_data.py: python coe to clean the data we have and create a database.

3) Models:
   - train_classifier.py: python code for Machine Learning Pipeline.
   - classifier.pkl: model that have been created will be saved here.

# Running the code:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_mespython datasages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/


# Credits

I have successfully completed this project, under the udacity nanodegree program, data science, below is the link to their website:
https://www.udacity.com/

In this project, Disaster Response Pipeline, the dataset is provided by Figure Eight, link to their website is given below:
https://appen.com/

# Screenshots of the working web app

![example of message classification(ss)](https://user-images.githubusercontent.com/72887048/125740712-7f0e7cb1-d247-4a1e-b1a0-39f752121684.png)


![uss4](https://user-images.githubusercontent.com/72887048/125740748-4577293c-ab1e-4c5a-8f75-ecad4ebf5648.png)







    
