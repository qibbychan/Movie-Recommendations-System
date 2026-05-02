🎬 **Hybrid Movie Recommendation System**
A hybrid recommendation engine that combines Content-Based Filtering and Collaborative Filtering to suggest movies based on both title similarity and user taste — built with an interactive UI inside Jupyter Notebook.

📖 Followed a project tutorial as the foundation, then focused on understanding every line of code, debugging real errors, and extending it with a custom genre filter feature.


📌 Problem Statement
Streaming platforms recommend millions of movies daily. How do they do it? This project explores two core recommendation strategies — matching movie content attributes and learning from user behaviour — then combines them into a single working system.

⚙️ How It Works
1. Content-Based Filtering

Uses TF-IDF to vectorize movie titles and metadata
Computes Cosine Similarity to find movies most similar to a given title
"If you liked Movie A, here are movies with similar attributes"

2. Collaborative Filtering

Identifies users with similar rating patterns
Recommends movies that similar users enjoyed
"Users who liked what you liked also enjoyed these..."

3. Interactive UI (Jupyter Widgets)

Real-time movie search with ipywidgets
Genre filter dropdown — added beyond the original tutorial
Results displayed dynamically without rerunning cells


💡 What I Actually Learned
Beyond following the tutorial, I actively debugged and extended the project:

Fixed NameError and SyntaxError issues by tracing through execution flow
Resolved NaN value problems in the similarity matrix during preprocessing
Added a genre filter feature not in the original tutorial
Gained a deep understanding of how TF-IDF and cosine similarity work together


🛠️ Tech Stack

Language: Python 3
Libraries: Pandas, Scikit-learn, ipywidgets, Jupyter Notebook
Dataset: movies.xls (included in repo)


📁 Project Structure
Movie-Recommendations-System/
│
├── Movie Recommendation Project.ipynb   # Main notebook with full system + UI
├── movies.xls                           # Dataset
└── README.md

🚀 How to Run
bash
# 1. Clone the repo
git clone https://github.com/qibbychan/Movie-Recommendations-System.git
cd Movie-Recommendations-System

# 2. Install dependencies
pip install pandas scikit-learn ipywidgets jupyter xlrd

# 3. Enable Jupyter widgets
jupyter nbextension enable --py widgetsnbextension

# 4. Launch the notebook
jupyter notebook "Movie Recommendation Project.ipynb"

🔮 Future Improvements

 Integrate with the TMDB API for live movie data and poster images
 Add a rating input so users can personalize recommendations
 Deploy as a Streamlit web app for public access
 Experiment with matrix factorization (SVD) for better collaborative filtering


🏷️ Topics
recommendation-system machine-learning collaborative-filtering content-based-filtering nlp python jupyter-notebook ipywidgets tfidf cosine-similarity
