# CineMatch-ML 🎬

A content-based movie recommendation system built using Python, Pandas, Scikit-learn, Streamlit, and the TMDB API.

## Project Overview

CineMatch-ML recommends movies similar to a movie selected by the user. It uses movie metadata and a similarity-based recommendation approach to suggest related movies along with their posters.

## Features

* Select a movie from the dropdown.
* Get recommendations for similar movies.
* Display movie posters using the TMDB API.
* Interactive web interface built with Streamlit.

## Technologies Used

* Python
* Pandas
* Scikit-learn
* Streamlit
* TMDB API
* Pickle

## Project Files

* `app.py` – Streamlit application and recommendation logic.
* `MRS_EDA.ipynb` – Exploratory data analysis and project notebook.
* `movie.pkl` – Movie data used by the application.
* `movie_dict.pkl` – Movie dictionary used by the application.
* `requirements.txt` – Python dependencies.

## How to Run Locally

1. Clone this repository:

   ```bash
   git clone https://github.com/pragyasingh7803/CineMatch-ML.git
   ```

2. Open the project folder:

   ```bash
   cd CineMatch-ML
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Configure your TMDB API key as an environment variable.

5. Run the application:

   ```bash
   streamlit run app.py
   ```

## Acknowledgements

Movie data is sourced from The Movie Database (TMDB).

This project is created for learning and demonstrating a content-based recommendation system.
