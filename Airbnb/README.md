## [Madrid Airbnb's dataset (Under construction)](../master/Airbnb)

### Introduction
As explained, I worked on an Airbnb dataset with information about reviews, locations, amenities and host’s descriptions in Madrid, where I was able to apply many tools I learned in that master.

In this project there were 3 main goals:

- Predict the price of a new airbnb apartment/room based on the amenities, description of the apartment/room and the location, providing as an additional information the prediction of the mean price in the neighborhood in the next 12 months.

- Classify the reviews with NLP and analyze and visualize the negative ones per neighborhood in order to detect issues and conflictive areas inside Madrid.

- Provide the guest information about public transport and points of interest near the selected apartment.

### Notebooks
I splited the whole project into different files in order to have access to them more easily.
The proper order of these files is:

1) [Dataset's creation](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/dataset_creation.ipynb): analysis of the features, feature engineering and data cleaning.
2) [Amenities' selection](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/amenities_selection.ipynb): deep analysis of one of the columns in the dataset, that contains the amenities in each apartment/room. In this notebook we define the significant amenities we should work with.
3) [Historical dataset's creation](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/historical_data.ipynb): to predict the price's evolution per Neighbourhood we need a dataset with the historical prices of the apartments and rooms in the original dataset. To create it, we scrapped all the csv files available in the airbnb's website and we merged all of them into one table.
After that we predict the price's evolution using Prophet.
4) [Price's recommendation](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/price_recom.ipynb): in this notebook we provide the recommended price of an apartment or room based on its characteristics. We provide the solution using Plotly.



