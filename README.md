# Content Based Movie Recommendation system

This repository contains a movie recommendation system that leverages natural language processing and machine learning techniques to recommend movies based on a user's plot search. The system uses a TF-IDF vectorizer to transform movie descriptions into numerical vectors and then calculates cosine similarities to find and rank movies that are most similar to the user's input.

## Dataset

The dataset used for this project is stored in a CSV file named titles.csv. This file contains movie titles, descriptions, genres, and production countries.

## Files

Movie_Recommendation.ipynb: Jupyter notebook containing the implementation of the movie recommendation system.

titles.csv: Dataset containing movie information.

# Requirements

+ Python3.6 or higher
+ TensorFlow
+ Pandas
+ Numpy
+ Scikit-learn
+ Seaborn
+ Matplotlib

You can install the required libraries using the following commands:

```sh
pip install tensorflow pandas numpy scikit-learn seaborn matplotlib
```

## Usage

```sh
git clone https://github.com/yash2010/Content_based_recommendation.git
```
## Functions

### _'description_vectorize(df, description)'_
+ Fills missing description values with an empty string.
+ Converts movie description into TF-IDF vectors.
+ Returns the TF-IDF matrix and the vectorizer.
### _'cos_sim(desc_data, desc_imput)'_
+ Computes the cosine similarity between each movie description and user's input.
+ Returns a list of similarity scores.
### _'top_n(n)'_
+ Sorts movies by similarity scores in descending order.
+ Returns the top 'n' most similar movies.

## Visualization
The notebook also generates a similarity heatmap for the top recommended movies using Seaborn's hearmap function. This heatmap visually represents the pairwise similarity scores between the top recommended movies.

## Example 
After running the notebook and entering a plot description, the system will output the top 5 movies that are most similar to the user's input and display a similarity heatmap.



  
 
