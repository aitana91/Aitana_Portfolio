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
2) [Amenities' selection](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/amenities_selection.ipynb): deep analysis of one of the columns in the dataset, that contains the amenities in each apartment/room. In this notebook the significant amenities we should work with are defined.
3) [Historical dataset's creation](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/historical_data.ipynb): to predict the price's evolution per Neighbourhood a dataset with the historical prices of the apartments and rooms in the original dataset is needed. To create it, I scrapped all the csv files available in the airbnb's website and  merged all of them into one table.
After that the price's evolution is predicted using Prophet.
4) [NLP in descriptions](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/nlp_descriptions.ipynb): the description column might be important when predicting the price, so I decided to apply NLP on the description column in order to use the BoW later.
5) [Price's recommendation and visualization](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/price_recom.ipynb): in this notebook the recommended price of an apartment or room based on its characteristics is predicted. The visual solution is provided using a [heat map](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/images/heat_map.PNG).
6) [Sentiment analysis of the reviews](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/sentiment_analysis.ipynb): the reviews are provided in a dataset with no classification (positive/negative or a punctuation). Therefore, a sentiment analysis is needed to perform this classification. After that, some Wordclouds are created.
7) [Negative reviews visualization](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/neg_reviews_plotly): two different visualizations are performed in Plotly:
    - the negative reviews are grouped based on the issue and are visualize in a [heat map](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/images/neg-topics.png). That way we can see if there are conflictive areas inside Madrid for each issue.
    - the location of the negative reviews are plotted by [neighbourhood](https://github.com/aitana91/Aitana_Portfolio/blob/master/Airbnb/images/neg-neig.png). That way we can see if there are conflictive areas inside each neighbourhood.


