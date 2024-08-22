# S&P 500 Predictor

The attatched Jupyter Notebook is a machine learning model trained to make educated predictions on the S&P 500 index

The Model is trained on data imported from Yahoo Finance giving us record to the S&P 500 index dating back to 1900. The data is then cleaned into what is needed and trained on predicting through a RandomForestClassifier. Using this, the Model takes the most recent 100 days and finds patterns/trends to predict if the index will go up or down on the next day. The model uses a 0/1 system assigning if the index has gone down(0) or up(1) and uses this to create an "precision score", aka accuracy. This Model produces an accuracy of 52.9%

Additionally, in the improvement section, the predict function is modified into a new function using probability instead. Rather than a 0 or 1 from before, we take the probability of 0.0-1.0 to assign our data trained. This slight modification shows a roughly 5% increase in the model.

The Model is tested through a back-testing system which allows for continuous improvement. Through the back-testing our predictions are run through 11 years of previous data to check our accuracy and allow to change the model to increase our accuracy.
