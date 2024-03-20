# YelpReview-Ratings

Explore Yelp Dataset

The contents of this repository were used to conduct exploratory data analysis on the Yelp dataset provided: https://www.yelp.com/dataset 
In this repository, there are 2 notebooks, one containing a segment of data cleaning and preprocessing tasks and another to conduct methods of topic modeling/predictive modeling on the datasets.

From the yelp dataset, the business, user and review files were used for this project. 

1. [Data Cleaning](https://github.com/kellychoy/YelpReview-Ratings/blob/main/data_cleaning.ipynb)

   This notebook explains the steps to clean the dataset and condense the data to only restaurants in California. The overall dataset was ~8.8GB so runtime did take a while but this step is important for efficiency for the remaining steps of the project. Filter the business file to California only and remove unimportant columns [(see overview pg 6)](https://github.com/kellychoy/YelpReview-Ratings/blob/main/YelpReview-Ratings%20Overview.pdf) for a record of columns to drop. Then merge the business file with the review file on "user_ID". Then merge this new file with the user's file on "user_ID" again to create 1 final dataset to use. In the end there is 211,749 rows x 31 columns

2. [Topic Modeling/Predictive Modeling](https://github.com/kellychoy/YelpReview-Ratings/blob/main/topic_modeling_step.ipynb)

   This notebook explains the steps to prepare for Latent Dirichlet Allocation (LDA) Topic Modeling and several predictive model analyses. Utilizing NLTK (Natural Language Toolkit), the text was preprocessed and tokenized. Stop words were also removed and I made sure all the content we were working with was in the same language - in this case, English. 
