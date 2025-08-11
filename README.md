# Movie Recommendation System Project

## Overview

This project involves building a movie recommendation system using the MovieLens dataset. The system utilizes movie metadata and user ratings to recommend similar movies based on user input. The project aims to provide personalized movie recommendations by analyzing user preferences and movie similarities.

## Data Sources

- **MovieLens Dataset:** [MovieLens 25M Dataset](https://files.grouplens.org/datasets/movielens/ml-25m.zip)

## Project Structure

1. **Data Collection:**
   - The project uses the MovieLens dataset, which includes movie metadata and user ratings.
   - The dataset is loaded into a Pandas DataFrame for analysis.

2. **Data Processing:**
   - Movie titles are cleaned to remove special characters for better text processing.
   - TF-IDF Vectorization is applied to the cleaned movie titles to create feature vectors.
   - Cosine similarity is used to find similar movies based on the feature vectors.

3. **Recommendation System:**
   - A search function allows users to input a movie title and find similar movies.
   - User ratings are analyzed to identify similar users and recommend movies they rated highly.
   - The system provides a list of recommended movies based on similarity scores.

## Data Description

### Movies Data
- `movieId`: Unique identifier for each movie.
- `title`: Title of the movie.
- `genres`: Genres associated with the movie.
- `clean_title`: Cleaned version of the movie title for text processing.

### Ratings Data
- `userId`: Unique identifier for each user.
- `movieId`: Unique identifier for each movie.
- `rating`: Rating given by the user to the movie.
- `timestamp`: Timestamp of the rating.

## Usage

To run the project, execute the Jupyter Notebook provided. The notebook will load the dataset, process the data, and allow users to input a movie title to receive recommendations.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- MovieLens for providing the movie dataset.
- Scikit-learn for machine learning tools and libraries.
- Pandas for data manipulation and analysis.
