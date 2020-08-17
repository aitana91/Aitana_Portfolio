# Aitana_Portfolio
Portfolio with projects I've been working on. All of them are written in Python.

## [Madrid Airbnb's dataset (Under construction)](../master/Airbnb)
As a final project of a master I did, I worked on an Airbnb dataset with information about reviews, locations, amenities and host’s descriptions in Madrid, where I was able to apply many tools learned in that master.

In this project there were 3 main goals:

- Predict the price of a new airbnb apartment/room based on the amenities, description of the apartment/room and the location, providing as an additional information the prediction of the mean price in the neighborhood in the next 12 months.

- Classify the reviews with NLP and analyze and visualize the negative ones per neighborhood in order to detect issues and conflictive areas inside Madrid.

- Provide the guest information about public transport and points of interest near the selected apartment.

## [Movie Recommendation's System](../master/movies)
Development of a basic recommendation system using Python and Pandas. 
In this case the recommendation is based on the movies that the user has watched. We will use the cosine simmilarity to find the most similar users and we will recommend the user the most watched movies among these similar users.

## [Richter's Predictor: Modeling Earthquake Damage](../master/Earthquakes)
Based on aspects of building location and construction, the goal is to predict the level of damage to buildings caused by the 2015 Gorkha earthquake in Nepal.

Result: micro-averaged F1 score = 0.7289

## [Credit Card Fraud Detection](../master/Fraud)
In this case, the goal is to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

The dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.
