# 🎬 CineMatch-ML
### Content-Based Movie Recommendation System

CineMatch-ML is a content-based movie recommendation system built using Python, NLP-based text processing, machine learning techniques, and Streamlit.

The application recommends five movies similar to a movie selected by the user. It uses movie metadata to identify similarities between movies and displays the recommended movies along with their posters fetched from The Movie Database (TMDB) API.

---

## 📌 Project Overview

The objective of this project is to build a movie recommendation system that helps users discover movies based on their preferences.

Unlike collaborative filtering systems that rely on user ratings or viewing history, this project follows a content-based recommendation approach.

Movies are recommended based on similarities in their content and metadata.

The recommendation system uses a precomputed similarity matrix to identify movies that are most similar to the selected movie.

---

## 🚀 Features

- Select a movie from an interactive dropdown.
- Recommend five similar movies.
- Content-based movie recommendation.
- NLP-based processing of movie metadata.
- Similarity-based movie ranking.
- Display movie posters using the TMDB API.
- Interactive web interface built using Streamlit.

---

## 🧠 Machine Learning & NLP Techniques

### 1. Content-Based Filtering

The recommendation system follows content-based filtering.

It recommends movies based on their content-related features rather than user ratings or viewing history.

Movies with similar content representations receive higher similarity scores and are recommended to the user.

### 2. NLP and Text Processing

Natural Language Processing techniques are used in the movie recommendation pipeline to process textual movie information.

Movie metadata provides textual information that can be used to represent movies as feature vectors.

These representations help the system identify similarities between movies.

### 3. TF-IDF (Term Frequency-Inverse Document Frequency)

TF-IDF is a text feature extraction technique used to convert textual information into numerical representations.

It assigns importance to terms based on their frequency within a document and across the collection of documents.

These numerical representations can be used to compare movie content.

### 4. Cosine Similarity

Cosine Similarity is used to measure the similarity between numerical movie representations.

It calculates the cosine of the angle between two feature vectors.

Movies with higher cosine similarity scores are considered more similar.

The similarity scores are used to rank movies and generate recommendations.

### 5. Recommendation Logic

The application loads the precomputed movie data and similarity matrix.

When a user selects a movie:

1. The selected movie is identified in the movie dataset.
2. Its corresponding similarity scores are retrieved.
3. Movies are sorted based on their similarity scores.
4. The selected movie itself is excluded.
5. The top five similar movies are returned.
6. Movie posters are fetched from the TMDB API and displayed in the application.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| Python | Programming language |
| Pandas | Data manipulation and processing |
| NLP | Processing textual movie information |
| TF-IDF | Text feature extraction |
| Cosine Similarity | Movie similarity calculation |
| Streamlit | Interactive web application |
| TMDB API | Fetching movie posters |
| Pickle | Loading precomputed movie data and similarity matrix |

---

## 📂 Project Structure

```text
CineMatch-ML/
│
├── app.py
├── MRS_EDA.ipynb
├── movie.pkl
├── movie_dict.pkl
├── similarity.pkl
├── requirements.txt
└── README.md
```

### File Description

- `app.py` - Streamlit application containing the recommendation logic and user interface.
- `MRS_EDA.ipynb` - Jupyter Notebook used for exploratory data analysis and model preparation.
- `movie.pkl` - Preprocessed movie data.
- `movie_dict.pkl` - Movie dictionary used by the application.
- `similarity.pkl` - Precomputed movie similarity matrix used to generate recommendations.
- `requirements.txt` - Python dependencies required to run the project.
- `README.md` - Project documentation.

---

## ⚙️ Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/pragyasingh7803/CineMatch-ML.git
```

### Step 2: Navigate to the Project Directory

```bash
cd CineMatch-ML
```

### Step 3: Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment on Windows:

```bash
.venv\Scripts\activate
```

### Step 4: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 5: Configure TMDB API

The application uses the TMDB API to retrieve movie posters.

Configure your TMDB API key as an environment variable before running the application.

Do not upload API keys or other secret credentials to GitHub.

### Step 6: Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 📊 Dataset

The project uses movie metadata from the TMDB 5000 Movies and Credits datasets.

The metadata is processed to generate movie representations and similarity scores used by the recommendation system.

---

## 🎯 Project Objective

The objective of CineMatch-ML is to demonstrate how NLP-based text processing and similarity-based machine learning techniques can be used to build an interactive content-based recommendation system.

The project combines data processing, feature extraction, similarity calculation, and application development into a complete movie recommendation workflow.

---

## 🙏 Acknowledgements

Movie metadata and poster information are sourced from The Movie Database (TMDB).

This project is developed for educational and machine learning portfolio purposes.
