# Recommendation (IBM)
In this project, four recommendation systems on real data, captured from IBM Watson Studio platform are investigated:
- Rank Based Recommendation.
- User-User Based Collaborative Filtering.
- Content Based Recommendations.
- Matrix Factorization. 

### Table of Contents

1. [Imported Libraries](#libraries)
2. [Files Descriptions](#files)
3. [Analysis Workflow](#analysis)


### Libraries  <a name="libraries"></a>
The following packages are used in conjunction with Anaconda distribution Python 3.0.

1. Pickle
2. Matplotlib
3. NLTK
4. NumPy
5. Pandas

## File Descriptions <a name="files"></a>

  - Recommendations (IBM).ipynb : The Jupyter notebook: showcases the analysis done in order to explore the dataset, the data preparation and wrangling as well as the building of recommendation engine. The notebook contains markdown cells to help with documentation of the steps.

 - Recommendation (IBM).html : For reference an HTML version of the notebook is also available.

The data folder contains the dataset from IBM Watson Studio platform.
It contains 3 files:

- articles_community.csv:  articles descriptive information 
- user-item-interactions.csv: users interactions with articles 

## Analysis Workflow  <a name="analysis"></a>

#### Exploratory Data Analysis
Before making recommendations of any kind, I explored the data to identify any missing values and data distribution. I cleaned and prepared the data for the analysis.

#### Rank Based Recommendations
To get started in building recommendations, I first identified the most popular articles simply based on users interaction. Since there are no ratings for any of those articles, it made sense to assume that articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

#### User-User Based Collaborative Filtering
In order to build better recommendations for the users of IBM's platform, I took a look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users.

#### Content Based Recommendations
Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. I utilized NLP to develop a content based recommendation system. This system goes through each article title and finds the most common words(related to a content) throughout all the available articles and recommends articles based on the sum of matched words in the title of an article and popularity.

#### Matrix Factorization
Matrix decomposition is used to predict new articles an individual might interact with.