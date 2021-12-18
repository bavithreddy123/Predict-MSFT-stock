# Predict-MSFT-stock
Project Overview
Pre-requisites

Knowledge in Python, REST API calls and Machine learning. An active Azure subscription. You may use the Azure for Students to get a subscription for free or else you can use Azure free account.

Route at a glance

    Downloading the MSFT stock database using the Yahoo finance API.
    Uploading the database to Azure Blob storage.
    Training the model on the data using Linear regression and creating a real-time inference endpoint via deployment on AKS Cluster.
    Triggering the ML pipeline run to retrain the model when DB in blob storage is modified.
    Building a web application that automates all the above processes and adds functionality to the user end.

Results

The app predicts the max value or High for MSFT stock, since we deployed real-time inference selecting the model trained on the ‘High’ column. The user can either use the stock parameters i.e Open, High, Close and Low from current market watch to predict the future max value of the MSFT stock or choose to provide inputs for the same in order to ignore the current trend. The website also shows the current state of the market i.e Open or Closed and shows the live value when the market is open. When the market is closed, Open, High, Low and Close values are shown and all predictions are based on the week-long database until market close.

![1-t_tT7X-zQIaG6S1lbKt6Yw](https://user-images.githubusercontent.com/84835408/146638686-3fa65771-7986-4cd6-be54-148822fac699.png)

![Screenshot (561)](https://user-images.githubusercontent.com/84835408/146638749-89612902-9b1e-4360-9e30-0dbf8785c279.png) 
                                          ML pipeline triggred by blob.
                                          


