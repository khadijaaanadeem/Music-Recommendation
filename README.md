
#  Music Recommendation System

This project is a **content-based music recommendation system** built with Python. The system suggests songs similar to a given input track by combining textual metadata (genre, artist, track name) with numeric audio features.

It demonstrates the use of **machine learning techniques** such as TF-IDF vectorization, feature scaling, and Nearest Neighbors modeling to build an end-to-end recommender pipeline.



##  Features

✅ **Content-Based Recommendations:**
Identifies similar songs based on metadata and numeric audio attributes.

✅ **Text Feature Engineering:**
Uses TF-IDF vectorization to encode textual information into numerical vectors.

✅ **Audio Feature Integration:**
Incorporates numeric audio features (e.g., tempo, loudness, speechiness, acousticness) to enhance similarity calculations.

✅ **Efficient Similarity Search:**
Leverages Nearest Neighbors modeling with cosine similarity for fast retrieval of recommendations.

✅ **Data Visualization:**
Generates clear plots of recommended songs using Matplotlib and Seaborn.


##  Technologies Used

* Python
* pandas & NumPy
* scikit-learn

  * TfidfVectorizer
  * StandardScaler
  * NearestNeighbors
* Matplotlib
* Seaborn



##  Dataset

The system uses the **TCC CEDs Music Dataset**, containing metadata and audio features of songs spanning approximately 100 years.


##  How to Use

1. **Load the dataset**
   Load and preprocess the data to combine text and numeric features.

2. **Vectorize Features**
   Apply TF-IDF encoding to text columns and standard scaling to numeric audio columns.

3. **Train Nearest Neighbors Model**
   Fit a cosine similarity model on the combined feature matrix.

4. **Get Recommendations**
   Input a song title and retrieve the top-N most similar tracks.

5. **Visualize Results**
   Display the recommendations in a bar chart for easy interpretation.

---

##  Example

```python
recommended_songs = get_recommendations('cry', data, nn, combined_matrix, top_n=10)
print(recommended_songs[['track_name', 'artist_name', 'genre']])
```
##  Future Improvements

* Incorporate lyrics and additional metadata for richer recommendations.
* Add collaborative filtering for personalized suggestions.
* Implement approximate nearest neighbors (e.g., FAISS) to improve scalability.
* Deploy as a web app using Streamlit or Flask.


##  Purpose

This project showcases **practical machine learning skills** in recommendation systems, including data preprocessing, feature engineering, and model building, applicable to real-world use cases like music or content recommendations.

If you’d like, I can help you customize this README further or format it for GitHub Markdown!
# Music-Recommendation
