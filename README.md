# Movie Recommendation System in Python

## Project Overview
This project is a simple Movie Recommendation System developed using Python and machine learning techniques. The main purpose of the system is to recommend movies to users based on the ratings given by other users.

The system analyzes user behavior and movie ratings and suggests movies that are similar to the ones a user has already liked or rated highly. The recommendation is generated using the K-Nearest Neighbors (KNN) algorithm.

## Objective
The objective of this project is to understand how recommendation systems work and how machine learning can be used to provide personalized suggestions to users.

The project focuses on:
- Understanding collaborative filtering
- Implementing a recommendation system using KNN
- Working with real movie rating datasets
- Analyzing user rating patterns

## Technologies Used
The project is implemented using the following tools and technologies:

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Scikit-Learn
- SciPy
- Matplotlib
- Seaborn

These libraries are used for data processing, machine learning, and visualization.

## Dataset
The project uses the MovieLens dataset which contains movie information and user ratings.

### ratings.csv
This file contains the ratings given by users to different movies.

Columns include:
- userId – unique id of the user
- movieId – unique id of the movie
- rating – rating given by the user
- timestamp – time when the rating was given

### movies.csv
This file contains details about movies.

Columns include:
- movieId – unique id of the movie
- title – name of the movie
- genres – type or category of the movie

## Working of the System

### Loading the Dataset
First, the ratings and movies datasets are loaded using the Pandas library.

### Data Analysis
Basic analysis is performed to understand the dataset such as:
- total number of users
- total number of movies
- total number of ratings

### Creating the User-Movie Matrix
A matrix is created where:
- rows represent movies
- columns represent users
- values represent ratings given by users

Since most users have not rated every movie, the matrix is very sparse. Therefore, a sparse matrix format is used to store the data efficiently.

### Applying the KNN Algorithm
The K-Nearest Neighbors algorithm is used to find similar movies based on user rating patterns.

Cosine similarity is used to measure how similar two movies are.

### Generating Recommendations
When a user selects or rates a movie, the system finds similar movies using KNN and recommends them to the user.

## How to Run the Project

1. Download or clone the repository.

2. Install the required Python libraries.

pip install numpy pandas scikit-learn matplotlib seaborn scipy

3. Open Jupyter Notebook.

jupyter notebook

4. Run the file:

Recommendation_System_in_Python.ipynb

The notebook will load the dataset, build the recommendation model, and display recommended movies.

## Future Improvements
This project can be improved by adding additional features such as:
- combining collaborative filtering with content-based filtering
- building a web interface using Flask or React
- adding movie posters and better visualization
- using deep learning based recommendation models

## Conclusion
This project demonstrates how machine learning techniques can be used to build a basic movie recommendation system. Similar systems are widely used in real-world platforms such as Netflix, Amazon, and Spotify to suggest relevant content to users based on their preferences.