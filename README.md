# **Movie Recommendation System**

This is a simple movie recommendation system built using Python and Streamlit. The system recommends movies based on their similarity to the selected movie. The similarity is calculated using cosine similarity on movie descriptions, genres, keywords, cast, and crew.

### Components

1. **Data Preprocessing**: The system preprocesses the movie data by cleaning, transforming, and extracting relevant features such as genres, keywords, cast, and crew.

2. **Feature Engineering**: It creates a unified set of 'tags' by combining movie descriptions, genres, keywords, cast, and crew. This helps in building a feature matrix for similarity calculation.

3. **Model Building**: Cosine similarity is used to measure the similarity between movies based on their tags. The model recommends movies that are most similar to the selected movie.

4. **Streamlit App**: The recommendation system is wrapped into a Streamlit web application. Users can select a movie from a dropdown menu and click a button to view recommended movies.

### File Structure

- **`movie_recommendation.py`**: Contains the Python code for preprocessing, model building, and recommendation functions.
- **`app.py`**: Streamlit web application code to interact with the recommendation system.
- **`tmdb_5000_movies.csv`**: Dataset containing movie details.
- **`tmdb_5000_credits.csv`**: Dataset containing movie credits.
- **`movies_dict.pkl`**: Pickled dictionary containing preprocessed movie data.
- **`similarity.pkl`**: Pickled similarity matrix for movie recommendations.

### Usage

1. Clone the repository.
2. Install the required libraries: `pip install -r requirements.txt`.
3. Run the Streamlit app: `streamlit run app.py`.
4. Select a movie from the dropdown menu and click 'Show Recommendation' to view recommended movies.

### Dependencies

- **Pandas**: For data manipulation and preprocessing.
- **NumPy**: For numerical operations.
- **Scikit-learn**: For cosine similarity calculation.
- **NLTK**: For text processing and stemming.
- **Streamlit**: For building interactive web applications.
- **Requests**: For making API requests to fetch movie posters.

### References

- The movie dataset used in this project is sourced from [TMDb (The Movie Database)](https://www.themoviedb.org/).
- Stemming technique is applied using NLTK's PorterStemmer.
- Cosine similarity calculation is done using Scikit-learn.

### Demo

![Screenshot 2024-03-03 at 10 40 51 PM](https://github.com/danishziasiddique/Movie-Recommendation-System/assets/82972335/6fae01d6-9700-4d6a-91ff-54e81233e980)

https://pictureperfect-movie-recommendation-system-danishziasiddique.streamlit.app/

- Use the above link to access the project.

### Future Improvements

- Implementing more advanced recommendation algorithms like collaborative filtering.
- Enhancing user interface with additional features like search, filters, and ratings.
- Optimizing model performance for larger datasets.

### Contributors

- Danish Zia Siddique

Feel free to contribute to the project by forking the repository and submitting pull requests.
