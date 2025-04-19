# Music-Recommendation-Algorithm
Audio Recommendation Algorithm - Basic Project

Background

Now that we’ve had experience with supervised learning algorithms, let’s shift our attention to unsupervised learning applications. Namely, we will analyze a dataset of songs, their lyrical features, and (optionally) their lyrical content in order to discover clusters. 

Within this project, we will take a look at a real dataset of songs from 1950 to 2011. 

This dataset contains a mix of lyrical and continuous variables pulled from a 2020 research paper titled Music Dataset: Lyrics and Metadata from 1950 to 2019. Review the list below to find out more about this datasets columns:

artist_name: The name of the artist

track_name: The name of the song

release_date: When this song was released

genre: The categorical genre of this song

lyrics: The pre-tokenized lyrics of this song. Disclaimer: note that as this is real-world data, lyrical content is often obscene. 

len:  The number of words in the lyrics of this song

dating: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with dating.

violence: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with violence.

world/life: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the world or life in general terms.

night/time: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do night-life or time.

shake the audience: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with provocative feeling.

family/gospel: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with family-oriented content or the gospel.

romantic: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with romantic feeling.

communication: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with communication (either in romantic terms or otherwise).

obscene: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with obscene content (money, rockstar-lifestyle, etc).

music: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with music (music about music, basically).

movement/places: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with movement or various locations.

light/visual perceptions: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the sun or other physical weather-related patterns.

family/spiritual: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the importance of family or spirituality.

sadness: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the importance of family or spirituality.

feelings: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with emotions, either positive or negative.

topic: The categorical label of lyrical content

age: A score from 0 to 1 expressing how “old” a song is from our perspective. 1 being the oldest, and 0 being the newest.


Within this project, you will create a comprehensive machine learning pipeline that satisfies the patterned steps of a classic machine learning project. This entails:

beginning with hypothesis formulation through EDA, 
completing data cleaning, pre-processing, & dimensionality analysis, 
and concluding with model generation, sample prediction, and a report.

Instructions

The following is a list of expected notebooks that should be included in your project:

Initial EDA
Your project should begin with a notebook where you perform univariate, bivariate, and multivariate exploratory analysis. 
Be sure to create relevant graphs that will help you formulate a hypothesis. 
Since we have no target variable to predict, these plots will purely explore the interactions between predictors. Get creative and think of different ways to explore this dataset!

Data cleaning, pre-processing, and dimensionality reduction
After completing your EDA, you should move forward with creating a notebook where you will clean and wrangle your dataset. This might include dropping null values, removing unnecessary columns, removing outliers, and potentially fixing incorrectly formatted data. 
Furthermore, if you notice that some of these columns have strong correlation and linearity, it would be best to drop these columns (note: for now it would be best to drop the “lyrics” column).
Save this dataframe as a new csv file to be used in the next step.


Model creation, hyperparameter search, and model evaluation
Once you have cleaned and reduced this dataset, we will then create a notebook where we will implement a KMeans Clustering or any other clustering algorithm of your choice on your training dataset.
After initial training, evaluate the best number of clusters using one of the cluster identification techniques.
After generating your clusters for each sample in your training dataset, save these cluster-labels as a new column in your dataframe and save this dataframe for further analysis.

New Sample Prediction
Finally, apply your trained machine learning algorithm on the following test dataset, in order to generate cluster labels for each new sample.
After generating these clusters, save these labels as a new column in your test dataset and save this subsequent dataframe for further analysis.

Report
To conclude this project, we should answer the following 5 questions in a separate document attached to your project:

Which insights did you gain from your EDA? Were any columns highly correlated? If so, name them.

How did you determine which columns to drop or keep? If your EDA informed this process, explain which insights you used to determine which columns were not needed. 

What was the optimal number of clusters in your cluster model? Explain how you determined this value.

Take a look at the respective songs that fell into your clusters. Describe these clusters in human terms to the best of your ability using the columns in your dataset (for example high-gospel songs, low-gospel songs, etc). Feel free to listen to these songs as well to get a sense of what nuance your algorithm picked up on.

Take a look at the clusters that your algorithm assigned to your test samples. Based on these clusters, which songs would you recommend to this user?



(OPTIONAL BONUS CHALLENGE) Lyrical Analysis If you’ve completed the previous 5 steps and would like an additional sentiment analysis challenge, complete the following steps
For this bonus challenge, you will create an additional notebook that contains a Word2Vec model to analyze the lyrical content of our “lyrics” column. Look back to previous Word2Vec models to get an ideal on how this will be done!
After training a Word2Vec model, get a list of vectors of the words used in this dataset, and reduce these vectors down to two components using PCA analysis.
Visualize your lyrics and their PCA components using a scatter-plot to note the lyrical content of your dataset.

FAQ

Should I gitignore my data again?
	
While this dataset is not too large, it’s generally advisable to omit data sets from your GitHub repositories. It would be a good idea to make another .gitignore where you ignore any data.

I don’t know how to make a KMeans model. Where do I look to find this out?
	
We provide links to the KMeans model. Check out the example code to get started. Also we recommend that you use Google to see how other data scientists implement these learning algorithms.

How do I implement hyperparameter tuning?

We provide links to both Grid & RandomizedSearch objects. Check out the example code provided, as well as your code from the previous week's labs for ideas.

Which model/hyperparameter tuning strategy do I choose?

This is your executive decision to make. Better yet, why don’t you try out both and see which one performs better?

Submission

Submit a link to your repository with all required notebooks and write ups by 4/20

We are primarily interested in seeing which ideas you took away from the previous weeks of unsupervised learning + word2vec modeling. 
