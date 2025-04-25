
# Audio Recommendation Algorithm 
real dataset of songs from 1950 to 2011 exploring lyrical features and apply unsupervised learning applications

### Dataset Description
a mix of lyrical and continuous variables pulled from a 2020 research paper titled Music Dataset: Lyrics and Metadata from 1950 to 2019.

- artist_name: The name of the artist

- track_name: The name of the song

- release_date: When this song was released

- genre: The categorical genre of this song

- lyrics: The pre-tokenized lyrics of this song. Disclaimer: note that as this is real-world data, lyrical content is often obscene. 

- len:  The number of words in the lyrics of this song

- dating: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with dating.

- violence: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with violence.

- world/life: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the world or life in general terms.

- night/time: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do night-life or time.

- shake the audience: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with provocative feeling.

- family/gospel: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with family-oriented content or the gospel.

- romantic: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with romantic feeling.

- communication: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with communication (either in romantic terms or otherwise).

- obscene: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with obscene content (money, rockstar-lifestyle, etc).

- music: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with music (music about music, basically).

- movement/places: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with movement or various locations.

- light/visual perceptions: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the sun or other physical weather-related patterns.

- family/spiritual: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the importance of 
family or spirituality.

- sadness: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with the importance of family or spirituality.

- feelings: A score from 0 to 1 expressing how likely it is that this song’s lyrics have something to do with emotions, either positive or negative.

- topic: The categorical label of lyrical content

- age: A score from 0 to 1 expressing how “old” a song is from our perspective. 1 being the oldest, and 0 being the newest.


### Project Goals

###### Initial EDA
begins with a notebook where you perform univariate, bivariate, and multivariate exploratory analysis. relevant graphs will help formulate a hypothesis. Since we have no target variable to predict, these plots will purely explore the interactions between predictors.

###### Data cleaning, pre-processing, and dimensionality reduction
clean and wrangle your dataset; This might include dropping null values, removing unnecessary columns, removing outliers, and potentially fixing incorrectly formatted data. Furthermore, if you notice that some of these columns have strong correlation and linearity, it would be best to drop these columns (note: for now it would be best to drop the “lyrics” column). save this dataframe as a new csv file to be used in the next step.

###### Model creation, hyperparameter search, and model evaluation
implement KMeans Clustering or any other clustering algorithm. After initial training, evaluate the best number of clusters using one of the cluster identification techniques. After generating your clusters for each sample in your training dataset, save these cluster-labels as a new column in your dataframe and save this dataframe for further analysis.

###### New Sample Prediction
apply your trained machine learning algorithm on the following test dataset, in order to generate cluster labels for each new sample. After generating these clusters, save these labels as a new column in your test dataset and save this subsequent dataframe for further analysis.

### Report
following 5 questions answered:

- Which insights did you gain from your EDA? Were any columns highly correlated? If so, name them.

- How did you determine which columns to drop or keep? If your EDA informed this process, explain which insights you used to determine which columns were not needed. 

- What was the optimal number of clusters in your cluster model? Explain how you determined this value.

- Take a look at the respective songs that fell into your clusters. Describe these clusters in human terms to the best of your ability using the columns in your dataset (for example high-gospel songs, low-gospel songs, etc). Feel free to listen to these songs as well to get a sense of what nuance your algorithm picked up on.

- Take a look at the clusters that your algorithm assigned to your test samples. Based on these clusters, which songs would you recommend to this user?

### Modules/Libraries

- Python 
- MatplotLib
- Scikit-Learn
- Pandas 