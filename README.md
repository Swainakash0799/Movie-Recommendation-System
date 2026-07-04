# Movie Recommendation System

🚀 An **End-to-End Machine Learning Project** that recommends movies based on content similarity using **Cosine Similarity** and deployed with **Streamlit**.

---

## 🌐 Live Demo

👉 https://movie-recommendation-system-0799.streamlit.app/


---

## 📌 Project Overview

This project builds a **Content-Based Movie Recommendation System** that suggests movies similar to a selected one by analyzing features like genres, keywords, cast, and crew.

It demonstrates a complete ML pipeline:

* Data preprocessing
* Feature engineering
* Model building
* Web app development
* Deployment

---

## 🧠 How It Works

1. **Data Collection**

   * TMDB 500 Movies Dataset
   * 📁Link: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

2. **Data Preprocessing**

   * Merged datasets (movies + credits)
   * Removed unnecessary columns
   * Handled missing values
   * Cleaned and normalized text

3. **Feature Engineering**

   * Combined:

     * Genres
     * Keywords
     * Cast (Top 3)
     * Crew (Director)
   * Created a **tags column**

4. **Vectorization**

   * Applied **TF-IDF Vectorizer**

5. **Similarity Calculation**

   * Used **Cosine Similarity** to compute similarity between movies

6. **Recommendation System**

   * Input: Movie name
   * Output: Top 5 similar movies

---

## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Streamlit**
* **Requests**
* **TMDB API**

---

## ⚙️ Project Structure

```
movie-recommendation-system/
│
├── app.py                # Streamlit application
├── movie_dict.pkl        # Preprocessed movie dataset
├── requirements.txt      # Dependencies
├── .gitignore
└── README.md
```

---

## 🚀 Deployment Strategy

Due to GitHub file size limits, the similarity matrix (`similarity.pkl`) is **not stored in the repository**.

Instead:

* Hosted externally (Hugging Face)
* Loaded dynamically at runtime using `requests`
* Cached using Streamlit for performance

---

## ▶️ Run Locally

### 1. Clone the repository

```
git clone https://github.com/Swainakash0799/Movie-Recommendation-System.git
cd movie-recommendation-system
```

### 2. Install dependencies

```
pip install -r requirements.txt
```

### 3. Run the app

```
streamlit run app.py
```

---

## 🎯 Features

* 🎬 Movie recommendation based on similarity
* 🔍 User-friendly search interface
* 🖼️ Movie posters via TMDB API
* ⚡ Fast response using cached similarity matrix
* 🌐 Deployed on Streamlit Cloud

---

## 🔥 Future Improvements

* Add **Collaborative Filtering**
* Hybrid recommendation system
* Improve UI (Netflix-style design)
* Add user login & personalization

---

## 🙌 Acknowledgements

* TMDB API for movie data and posters
* Streamlit for web app deployment
* Scikit-learn for ML utilities

---




