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

![Screenshot (563)](https://user-images.githubusercontent.com/84835408/146638863-934f09f2-d3fd-4001-8d3d-5ae9927fedc8.png)

![Screenshot (561)](https://user-images.githubusercontent.com/84835408/146638749-89612902-9b1e-4360-9e30-0dbf8785c279.png)
                                   ML pipeline triggred by blob.
![Screenshot (564)](https://user-images.githubusercontent.com/84835408/146638974-85368dd1-884b-469e-b4b4-25d222b2866e.png)
                                          Pipeline Flow.
![Screenshot (565)](https://user-images.githubusercontent.com/84835408/146639118-b08aa8a6-8cc3-420a-b425-db3ff8c9966d.png)
                                       Experiments of pipeline flow/model 

