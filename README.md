# Data Cleaning and Story

The dataset comes from a kaggle.com competition and has already been cleaned for the most part.  It contains codings for the categorical data such as product name, department name and aisle name etc.  The orders are split into 3 parts known as train, test and prior.  This should be sufficient to develop machine learning algorithms for recommendations.

A few things I did to better understand and relate the data are worth noting.  A future assignment will incorporate these items in to a data story.

- Read in the csv files in to dataframes and reviewed basic details regarding column names and relatable fields.

- Combined the arrays by merging such that I had a complete definition of product, aisle, department and the associated codings. 

- Determined # of products

- Defined a dictionary to translate the days of the week from numbers to text to be used in future plots

- Defined a list of day order such that plots could be indexed appropriately

- Made use of a lambda function to map the dictionary to the dataframe and create a new column that could be called upon in the future

- Filled in empty cells with the mean value of days since prior order

- used the .head(), .info() and .describe() methods to better understand the dataframes

- the raw data comes with a column 'reorderd' that indicates whether or not the user bought the same product again.  In order to make this meaningful I had to create a new dataframe that put this in terms of each department and product as '%reordered'.

- took the mean of reordered by product and excluded items that were purchased a small number of times, <40

After making these changes and additions to the dataset I feel prepared to gain insights that will support the objective of developing a model to predcit purchases.

