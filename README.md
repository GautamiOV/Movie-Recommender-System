# Movie-Recommender-System
# 🎬 Movie Recommender System using Machine Learning & NLP

This project is a **Content-Based Movie Recommender System** that suggests similar movies based on user input. It applies **Natural Language Processing (NLP)** techniques and **Machine Learning** to analyze features like genres, cast, crew, keywords, and overview, enabling it to generate relevant recommendations. The project is implemented in **Python** using **Jupyter Notebook**.

---

## 📌 Project Objectives

- Build a movie recommender system using content-based filtering
- Use NLP techniques to process textual features of movies
- Create a similarity matrix using cosine similarity
- Provide top N movie recommendations based on a selected title
- Practice end-to-end feature engineering and model building using real-world data

---

## 🗂️ Dataset

- Source: [TMDB 5000 Movie Dataset (Kaggle)](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- Files used:
  - `movies.csv`
  - `credits.csv`

The dataset contains metadata on 5000+ movies, including:
- Title, Overview, Genres
- Keywords, Cast, Crew
- Popularity, Release Date, and more

---

## ⚙️ Tech Stack & Libraries

- **Python**
- **Jupyter Notebook**
- **Pandas** – Data manipulation
- **NumPy** – Array operations
- **Scikit-learn** – TF-IDF Vectorizer, Cosine Similarity
- **NLTK (optional)** – Text preprocessing
- **Ast, JSON** – Parsing complex nested columns

---

## 🧠 Project Workflow

1. **Data Preprocessing**
   - Merged `movies.csv` and `credits.csv` datasets
   - Extracted relevant features: title, overview, genres, cast, crew, and keywords
   - Parsed stringified columns using `ast.literal_eval()`
   - Extracted top 3 actors, director, and keyword tokens

2. **Text Normalization**
   - Combined features into a new column: `tags`
   - Lowercased and removed whitespace for uniformity
   - Stemming (optional step using NLTK’s PorterStemmer)

3. **Feature Extraction**
   - Applied `TfidfVectorizer` to transform tags into numerical features
   - Calculated **Cosine Similarity** between all movies

4. **Recommendation System**
   - Created a function `recommend(movie_title)` to return top 5 similar movies
   - Suggestions are based on vector similarity from the preprocessed features

---

## 💡 Key Features

- ✅ Real-world movie dataset with rich metadata
- ✅ Combined NLP and ML for content-based filtering
- ✅ Cosine similarity-based ranking
- ✅ Clean, modular, and reproducible notebook

---

## 🧠 Skills Demonstrated

| Skill | Description |
|-------|-------------|
| **Python** | Clean, modular code for end-to-end pipeline |
| **Data Cleaning** | Merged datasets, parsed JSON, handled missing values |
| **NLP** | Feature extraction from text (overview, genres, cast, crew, etc.) |
| **Scikit-learn** | TF-IDF Vectorization and Cosine Similarity |
| **Feature Engineering** | Combined multiple features into meaningful tags |
| **Recommendation Logic** | Built similarity matrix and ranked suggestions |

---

## 📂 Project Structure

movie-recommender-system/
├── movie_recommender.ipynb # Jupyter Notebook (Main source code)
├── README.md # Project documentation
├── data/
│ ├── movies.csv
│ └── credits.csv


---

## 🚀 How to Run This Project

### Requirements

- Python 3.8+
- Jupyter Notebook

### Install Dependencies

```bash
pip install pandas numpy scikit-learn
Run the Notebook
Download or clone the repository

Open movie_recommender.ipynb in Jupyter Notebook

Run all cells

Use the recommend("Movie Title") function to get suggestions

📌 Sample Output
python
Copy
Edit
recommend("The Dark Knight")
➡️ Output:

markdown
Copy
Edit
1. Batman Begins
2. The Dark Knight Rises
3. Man of Steel
4. Superman Returns
5. Watchmen
🙋‍♀️ About Me
I'm a Data Analyst with a growing skillset in Machine Learning and NLP. I enjoy building smart applications that solve real-world problems with data.

📫 Email: ovgautami258@gmail.com
