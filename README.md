# MOVIEVERSE-Movie-Recommendation-System
At some point each one of us must have wondered where all the recommendations that Netflix, Amazon, Google give us, come from. We often rate products on the internet and all the preferences we express and data we share (explicitly or not), are used by recommender systems to generate, in fact, recommendations. The two main types of recommender systems are either collaborative or content-based filters. In this project we use a Content-Based Recommender System that recommends movies similar to the movie user likes. The dataset used to build this model is taken from kaggle. The frontend is made using StreamLit framework.
## Steps Involved are:
### Gather the data
The dataset has been taken from kaggle which includes top 5000 movies according to their tmdb ratings.
### Data Cleaning
Data cleaning is done by selection of the columns that plays an important role in forming a recommendation and by fetching the relevant data. For example:  Everything needs to be lowercase to avoid duplications, and I also decided to merge all first and last names in one unique word. 
### Modeling
In order to detect similarities between movies, we need to vectorize. **Vectorization** is a technique to implement arrays without the use of loops. Once we have the matrix containing the count for each word, we can apply the cosine-similarity function. At this point, we can write the actual function that takes a movie title as input, and returns the top 5 similar movies.
### Fronend using StreamLit
Front-End of the system is pretty simple made using streamlit app framework.
