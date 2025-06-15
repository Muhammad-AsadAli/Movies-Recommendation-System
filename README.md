# 🎥 Movie Recommendation System

This project is a **content-based movie recommendation system** that suggests movies similar to the one you like. It looks at things like genres, cast, crew, and plot summaries to figure out which movies are most alike—without relying on user ratings or reviews.

## 📚 About the Dataset

The data comes from the [TMDB 5000 Movie Dataset on Kaggle]. It includes:

- `movies.csv` — basic movie details like title, genres, overview, etc.
- `credits.csv` — information about the cast and crew.

These two files are merged and cleaned up to create a solid base for the recommendation engine.

## 🔍 How It Works

Here’s a quick breakdown of the process:

1. **Data Preprocessing**  
   Clean the data and combine relevant features like genre, cast, director, and keywords.

2. **Text Vectorization**  
   Create a combined “tag” for each movie and convert it into numerical vectors using `CountVectorizer`.

3. **Similarity Calculation**  
   Use cosine similarity to measure how close each movie is to the others based on their content.

4. **Recommendation**  
   When you input a movie title, the system finds the top 5 most similar movies and recommends them.

## 🛠️ Tools & Libraries

- Python
- Pandas & NumPy
- Scikit-learn
- NLTK (for text processing)
- Jupyter Notebook

## 💡 Example

Say you search for:  
```python recommend("Avatar")`
You might get results like:

John Carter

Guardians of the Galaxy

Interstellar

Ender's Game

Gravity
