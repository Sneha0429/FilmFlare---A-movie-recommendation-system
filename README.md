# 🎬 FilmFlare – Movie Recommendation System

FilmFlare is a content-based movie recommendation system that suggests similar movies using cosine similarity and metadata from The Movie Database (TMDB).  
The project is built using **Python, Streamlit**, and a trained ML model stored in `.pkl` files.

---

## 🚀 Features

- Recommend top 5 similar movies based on user selection  
- Fetch movie posters dynamically from TMDB API  
- Simple, clean UI using Streamlit  
- Lightweight & fast response  
- Pre-processed model files for instant predictions

---

## 🧠 Tech Stack

| Component | Technology |
|----------|------------|
| Web App | Streamlit |
| ML Model | Cosine Similarity |
| Programming Language | Python |
| Dataset | TMDB Movies 5000 dataset |
| API | TMDB API |

---

## 📂 Project Structure

```bash
Movie Recommendation System/
│── app.py
│── README.md
│── .gitignore
│
├── model/
│ ├── movie_list.pkl
│ ├── similarity.pkl
```

---

## ⚠️ Important Note About PKL Files

GitHub does **NOT** allow uploading files larger than 100 MB.  
The file `model/similarity.pkl` is around **176 MB**, so it cannot be stored in the repository.

👉 Therefore, users must **download the PKL files separately** and place them in the `model/` folder manually.

---

## 📥 Download Model Files (PKL)

### **Download Link (Google Drive)**
🔗 *Add your Google Drive link here after uploading:*  
`https://drive.google.com/...`

Users should:

1. Download **movie_list.pkl**  
2. Download **similarity.pkl**  
3. Create a folder named `model/` in the project  
4. Put BOTH files inside the folder:

```bash
model/
│── movie_list.pkl
│── similarity.pkl
```


---

## 🔑 TMDB API Key Setup

FilmFlare uses **TMDB REST API** to fetch posters.

Follow these steps:

1. Create an account → https://www.themoviedb.org/signup  
2. Verify your email  
3. Go to API settings → https://www.themoviedb.org/settings/api  
4. Request a **Developer API Key**  
5. Copy your key  
6. Replace the API key inside `app.py`:

```python
url = f"https://api.themoviedb.org/3/movie/{movie_id}?api_key=YOUR_API_KEY&language=en-US"
```

## ▶️ How to Run the Project Locally

### 1. Install Python (3.10+ recommended)

Download from: https://www.python.org/downloads/

### 2. Install Required Libraries

Run:
```python
pip install streamlit requests pickle5 pandas numpy
```
### 3. Place the PKL Files

- Create a folder named model

- Place the downloaded files inside:

Run:
```python
model/movie_list.pkl
model/similarity.pkl
```
### 4. Run Streamlit App

Use:

Run:
```python
python -m streamlit run app.py
```

## 🖥️ Screenshots

### Add screenshots here later

