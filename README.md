# 🎬 Movie Recommendation System

A machine learning-based movie recommendation system developed for an OTT platform to provide personalized movie suggestions based on users' recently watched movies. The project compares **Word2Vec** and **Sentence Transformer** embeddings and uses **Cosine Similarity** to identify similar movies.

## 📌 Project Overview

The existing recommendation system may not always match individual user preferences effectively. This project analyzes **11 months of viewing history** and develops an AI-based recommendation approach to improve personalization, user engagement, customer satisfaction, and overall content consumption.

## 🎯 Objectives

* Provide personalized movie recommendations.
* Identify movies similar to a user's viewing history.
* Compare **Word2Vec** and **Sentence Transformer** approaches.
* Evaluate recommendation performance using success rates.
* Build an interactive interface for generating movie recommendations.

## 🗂️ Dataset

### Movie Data

* **title** – Name of the movie.
* **genres** – Genres associated with the movie.
* **overview** – Short description of the movie storyline.

### Evaluation Data

* **movie_1 to movie_7** – Recently watched movies.
* **date** – Recommendation/evaluation date.
* **movie_watch** – Movie actually watched after recommendation.
* **past_success** – Indicates whether the previous recommendation was successful.

## 🧠 Methodology

### 1. Word2Vec

Movie information is processed and converted into vector representations using **Word2Vec**. Average embeddings of recently watched movies are calculated and compared with other movies using cosine similarity.

### 2. Sentence Transformer

The project uses the **`all-MiniLM-L6-v2`** Sentence Transformer model to generate semantic embeddings from:

* Movie title
* Genres
* Movie overview

The average embedding of recently watched movies is compared against all movie embeddings to generate the **Top 10 recommendations**.

### 3. Model Evaluation

Both approaches are evaluated by checking whether the movie actually watched by the user appears in the generated recommendations.

The project also analyzes recommendation **success rates across different months**.

## 🚀 Recommendation Workflow

```text
User's Recently Watched Movies
              ↓
      Movie Information
              ↓
       Text Embeddings
        ↙           ↘
    Word2Vec    Sentence Transformer
        ↘           ↙
       Cosine Similarity
              ↓
       Top 10 Recommendations
              ↓
       Model Evaluation
```

## 💻 Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Word2Vec
* Sentence Transformers
* Matplotlib
* Gradio

## 🖥️ Interactive Interface

A **Gradio-based interface** is implemented where users can select up to three movies they have watched. The system then generates a list of recommended movies using the Sentence Transformer model.

## ⭐ Key Features

* Personalized movie recommendations
* Semantic movie similarity
* Word2Vec-based recommendations
* Sentence Transformer-based recommendations
* Cosine similarity
* Recommendation success-rate analysis
* Monthly performance analysis
* Interactive Gradio interface

## 📊 Model Comparison

The project compares **Word2Vec** with **Sentence Transformer** embeddings to determine which approach provides more effective movie recommendations.

Based on the project evaluation, **Sentence Transformer performed better and was selected for the interactive recommendation interface**.

## 🎯 Business Impact

The recommendation system is designed to:

* Improve user experience.
* Increase recommendation relevance.
* Reduce the effort required to find movies.
* Improve user engagement.
* Encourage higher content consumption.

## 🔮 Future Enhancements

* Add collaborative filtering.
* Incorporate user ratings and watch history.
* Build a hybrid recommendation system.
* Deploy the application as a web application.
* Add movie posters, ratings, and additional metadata.
* Improve recommendations using larger datasets and advanced transformer models.

## 👩‍💻 Project

**Movie Recommendation System – AI/ML Project**

Developed using Python, NLP, embedding techniques, and machine learning to create personalized movie recommendations.
