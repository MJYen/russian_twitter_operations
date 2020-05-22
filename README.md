# Tracking State Information Operations on Twitter

## Project Summary
Social media has become the battlefield for the hearts and minds of various population groups around the world. World superpowers have recognized the benefits of using social media to project their soft power efforts and dedicated a considerable amount of resources towards conducting information operations in the digital space. In 2014, the notorious operation conducted by the IRA (Internet Research Agency), a Russian company involved in influence operations, led to 3,841 Twitter accounts being shut down. However, the media channels owned by the Russian Federation (RT, Sputnik, Ruptly) continue to thrive on Twitter and have amassed a rather large following. Is Russia still attempting to influence the American population? What narratives is Russia most interested in propagating?

To answer these questions, the project will investigate the narratives being propagated by the Russian media on Twitter, illuminate networks of social media users, and detect users enabling message propagation through networks and the use of bot-nets.

## Data

1. <b>Twitter Data Set - </b>Twitter accounts of major Russia-owned media (RT, Sputnik, Ruptly) and users in their network (users who interact with the content)

2. <b>Russian State Owned Media Websites - </b>Article text linked to in Tweets by RT, Sputnik, Ruptly

## Data Manipulation
### Initial Processing
* The data processing for the initial set of data from the Twitter API would enable identification of the network of users interacting with the content. This will be done through reading the 3,200 tweets per agency available from the API into Pandas DataFrames and the extraction of mentions, comments, and likes. Vectorized operations will be performed on the DataFrames whenever possible to aid algorithmic efficiency.
* The follow-on data processing will yield a network of users and their activity levels. This extraction will allow us to map out the user network and illuminate the dissemination of messages propagated on Russia-funded media accounts. Additionally, the data set would likely reveal the use of bot-nets for message propagation.
* The processing of the articles’ text shared through URL on Twitter will yield topics through Natural Language Processing (NLP) topic modeling involving the nltk library.
### Combining the Datasets
* The combination of the two datasets will allow us to encode nodes with topics extracted through the topic modeling and to size the edges by traffic, thus visualizing the key nodes in the network. Network centrality measures would reveal the most influential nodes in the network and key nodes connecting various communities.

## Visualizing the Results
One of the visualizations we will be creating will be a network visualization of narratives propagated by the state. The visualization would combine information from both the Twitter API (the content of the tweets) as well as the article text, which would be used in identifying the narrative topics being propagated.

## Contributors
Viktor Avdulov; Viktor will be responsible for obtaining data from Twitter API and preparing the data for visualization. Additionally, Viktor will combine the data sources and visualize the overlap of the data sets.

Tyvand McKee; Tyvand will be responsible for mapping out the network of users and activity levels. He will also work on the visualization that combines the datasets.

Monica Yen; Monica will be responsible for the processing of article text through web scraping and NLP topic modeling.
