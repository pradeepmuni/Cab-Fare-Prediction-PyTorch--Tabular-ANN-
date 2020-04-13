# Cab-Fare-Prediction-PyTorch--Tabular-ANN-
Modeled a Tabular Artificial Neural Network using PyTorch (fast.ai library) to predict the cab fares in New York city and performed various Feature Engineering tasks to convert the GPS coordinates into it’s equal distance using haversine and extracted information from timestamp to create new features. Implemented Feature encoding, Dropout, Embeddings to the model to get the best accuracy score of 95% with RMSE Loss of 3.3324



The <a href='https://www.kaggle.com/c/new-york-city-taxi-fare-prediction'>Kaggle NYC Taxi Fares </a> provides a dataset with about 55 million records. The data contains only the pickup date & time, the latitude & longitude (GPS coordinates) of the pickup and dropoff locations, and the number of passengers. It is up to the contest participant to extract any further information. For instance, does the time of day matter? The day of the week? How do we determine the distance traveled from pairs of GPS coordinates?

For this we've whittled the dataset down to just 60,000 records from April 11 to April 24, 2010. The records are randomly sorted. We'll calculate distance from GPS coordinates by using <a href='https://en.wikipedia.org/wiki/Haversine_formula'>haversine formula</a> and also extract the information like day of the week, am vs. pm, etc. as a part of Feature Engineering
