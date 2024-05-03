
# Book Recommendation System

This is a book recommendation system that provides recommendations based on popularity and collaborative filtering.


## Getting Started

1. Clone the repository: git clone https://github.com/NirzariP/Books-Recommendation-System.git
2. Install the required libraries
3. Download the dataset files (books.csv, users.csv, ratings.csv) and place them in the project directory.
## Datasets

The dataset used for this project includes three CSV files: books.csv, users.csv, and ratings.csv. These files contain information about books, users, and ratings, respectively.
## Libraries Used

numpy, pandas, pickle, cosine_similarity
## Usage/Examples
Popularity Based Recommendations:
The popularity-based recommender system recommends books based on their popularity among all users.
```python
import pickle

# Load the popularity-based recommender data
popular_df = pickle.load(open('popular.pkl', 'rb'))

# Display the top recommended books
print(popular_df.head())
```

Collaborative Filtering Based Recommendations:
The collaborative filtering-based recommender system recommends books based on user similarities.
```python
import pickle

# Load the collaborative filtering data
pt = pickle.load(open('pt.pkl', 'rb'))
similarity_scores = pickle.load(open('similarity_scores.pkl', 'rb'))

def recommend(book_name):
    # Function to recommend books based on user similarities
    pass

# Example usage
recommend('1984')
