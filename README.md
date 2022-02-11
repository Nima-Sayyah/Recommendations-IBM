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

The files structure is arranged as below:

    - README.md: read me file
	
    - Recommendation (IBM).ipynb: contains main analysis workflow

          > Exploratory Data Analysis
          > Rank Based Recommendations
          > User-User Based Collaborative Filtering
          > Content Based Recommendations
          > Matrix Factorization
          > Extras & Concluding
	
    - Recommendation (IBM).html: HTML version of the notebook as a reference
	
    - \Data (IBM Watson Studio datasets)
	        
          - articles_community.csv:  articles descriptive information 
          - user-item-interactions.csv: users interactions with articles  

## Analysis Workflow  <a name="analysis"></a>

#### Exploratory Data Analysis
I initially explored the data to identify any missing values and data distribution. I then cleaned and prepared the data for the analysis.

#### Rank Based Recommendations
I identified the most popular articles based on the users interaction. As there are no ratings for any of those articles, the assumption was then made that the most popular articles are the most intracted ones. These articles could then be recommended to new users.

#### User-User Based Collaborative Filtering
To build better recommendations for the users I explored similar users in terms of the items they have interacted with. These items can then be suggested to the similar users. This is a fine approach twoards personal recommendations for the users.

#### Content Based Recommendations
There are various ways with which someone opt to implement a content based recommendations system. I utilized **NLP** to develop a content based recommendation system. This system scans each article title and finds the most common and relevant words in all the available articles. The recommendation engines then selects the articles based on the sum of matched words in the title of an article in conjunction with popularity.

#### Matrix Factorization
Matrix factorization is a class of collaborative filtering algorithms used in recommender systems.  Its algorithms work by decomposing the user-item interaction matrix. Therefore, I used, **Singular Value Decomposition** (**SVD**) for that purpose to predict new articles an individual might interact with.

## Licensing, Authors, Acknowledgements, etc.
Acknowledgement should go to Udacity for the project inspiration.