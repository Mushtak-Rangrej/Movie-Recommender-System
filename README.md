# 🎬 Movie Recommender System

An interactive **Movie Recommender Web App** built with **Python** and **Streamlit** that suggests movies based on your favorite selection using a **content-based filtering** approach.

This app uses data from the TMDB 5000 Movie Dataset and provides movie posters via the TMDb API.

🚀 Features

- 🔍 Content-Based Movie Recommendations
- 🖼️ Movie posters fetched using **TMDb API**
- 🧠 Uses **cosine similarity** to recommend similar movies
- 🎨 Built with **Streamlit** for a clean and responsive UI
- 📦 Includes pickled model and preprocessed data for fast performance

📂 Project Structure

 app.py # Streamlit app file
 Movie Recommender.ipynb # Jupyter Notebook for development/testing
 movies_dict.pkl # Pickled DataFrame containing movie metadata
 similarity.pkl # Pickled similarity matrix
tmdb_5000_movies.csv # Raw movie metadata
 tmdb_5000_credits.csv # Cast & crew data
 Movie Recommender SS.pdf # Screenshot of the application
 README.md # This file

🧰 Technologies Used

- **Python**
- **Streamlit**
- **Pandas**
- **Scikit-learn**
- **Pickle**
- **Requests**
- **TMDb API**

---

 📦 Installation & Run Locally

1. Clone the repository
```bash
git clone https://github.com/yourusername/movie-recommender-streamlit.git
cd movie-recommender-streamlit
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt

You can create requirements.txt with:
bash
Copy
Edit
pip freeze > requirements.txt

Run the app
streamlit run app.py

⚙️ How It Works
Loads a precomputed similarity matrix using cosine similarity based on textual features like genres, keywords, cast, etc.

Displays a dropdown menu of available movies.

On selection, shows the top 5 most similar movies with poster images fetched dynamically from TMDb API.

🔑 API Key Info
To use the TMDb API (for fetching posters), an API key is embedded in the code:

python
Copy
Edit
https://api.themoviedb.org/3/movie/{movie_id}?api_key=YOUR_API_KEY
You can get your own key by creating a free account at TMDb.

Add a search bar with fuzzy matching

Allow filtering by genre, release year, or actors


📄 License
This project is licensed under the MIT License.

🙌 Acknowledgements
TMDb API

Streamlit

Kaggle - TMDB 5000 Movie Dataset


📸 Screenshot
![Demo of Movie Recommender Sytem](https://github.com/user-attachments/assets/fa15568d-e90e-4d96-9d6e-02e1fea02365)


