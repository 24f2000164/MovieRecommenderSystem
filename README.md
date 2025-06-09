# 🎬 Movie Recommender System

A simple and interactive **Movie Recommender System** built using **Streamlit**. It provides movie recommendations based on content similarity from a precomputed matrix.

---

## 🚀 Features

- 🎯 Content-based recommendation engine  
- ⚡ Fast response using precomputed similarity matrix  
- 🖥️ Web interface with Streamlit  
- 🌐 Ready for deployment on Render/Heroku

---

## 📁 Project Structure

```
├── app.py                  # Main application file
├── movies_dict.pkl         # Movie data dictionary
├── similarity.pkl          # Precomputed similarity matrix
├── requirements.txt        # List of dependencies
├── setup.sh                # Streamlit server configuration
├── Procfile                # Deployment instructions for Heroku/Render
└── README.md               # Project documentation
```
🛠️ Installation & Setup

1. Clone the Repository

git clone https://github.com/24f2000164/MovieRecommenderSystem.git
cd movie-recommender

2. Install Required Packages
 Make sure Python 3.8+ is installed. Then run:


```pip install -r requirements.txt```


 3. Run the App Locally
```streamlit run app.py```

How It Works
Loads the movie dataset and similarity matrix from .pkl files.

Uses cosine similarity or other distance metrics to find movies similar to the selected one.

Recommends top 5 similar movies.

Optionally displays movie posters (via TMDB API if integrated).

📦 Dependencies
All dependencies are listed in requirements.txt. Key ones include:

streamlit

pandas

numpy

pickle

pydeck

requests

altair

Deployment Guide (Render/Heroku)

1. setup.sh
   ```mkdir -p ~/.streamlit/
echo "\
[server]\n\
port = \$PORT\n\
enableCORS = false\n\
headless = true\n\
" > ~/.streamlit/config.toml```

2. Procfile
   web: streamlit run app.py --server.port=$PORT --server.enableCORS false


3. Deploy
Push to GitHub and deploy via Render or Heroku using their UI.

👤 Author
Sahil Kumar
📧 bt23ece015@nituk.ac.in
🔗 [Linkedin](https://www.linkedin.com/in/sahil-kumar-1645a3324?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BsZ9%2BLcdJRjif4SB7%2FFO1%2BQ%3D%3D)
💻  [Github](https://github.com/24f2000164/)

📄 License
This project is licensed under the MIT License.
Feel free to use and modify it for your own projects!
