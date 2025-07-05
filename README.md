#  Music Recommendation System (Spotify Tracks Dataset)

This project is a **Content-Based Music Recommendation System** built using the [Spotify Tracks Dataset (1921–2020)](https://www.kaggle.com/datasets/zaheenhamidani/ultimate-spotify-tracks-db). It recommends songs based on audio features such as danceability, energy, acousticness, valence, tempo, and more — similar to how platforms like Spotify suggest new music.

---

##  Dataset Overview

The dataset contains over **160,000 tracks** with the following features:

| Column | Description |
|--------|-------------|
| `genre` | Genre of the track (Pop, Rock, etc.) |
| `artist_name` | Name of the artist or band |
| `track_name` | Name of the track |
| `track_id` | Unique Spotify ID |
| `popularity` | Popularity score (0–100) |
| `acousticness` | Confidence that the track is acoustic (0.0–1.0) |
| `danceability` | How suitable a track is for dancing |
| `duration_ms` | Track length in milliseconds |
| `energy` | Intensity and activity level |
| `instrumentalness` | Likelihood of no vocals |
| `key` | Musical key (0 = C, ..., 11 = B) |
| `liveness` | Presence of audience (live performance) |
| `loudness` | Overall loudness in dB |
| `mode` | Major (1) or minor (0) modality |
| `speechiness` | Presence of spoken words |
| `tempo` | Tempo in BPM |
| `time_signature` | Estimated time signature |
| `valence` | Musical positivity or mood (0.0–1.0) |

---

##  Project Features

-  Content-Based Recommendation (no user data required)
-  Uses audio features to find similar songs
-  Efficient memory usage with `NearestNeighbors` (avoids memory errors)
-  Scalable to large music libraries
-  Simple and reusable function for real-time recommendations

---

## Technologies Used

- Python 
- Pandas
- NumPy
- Scikit-learn (StandardScaler, NearestNeighbors)
- Jupyter Notebook (for prototyping)

---

##  How It Works

1. **Feature Selection & Scaling**:  
   Key audio features are selected and normalized using `StandardScaler`.

2. **Model Building**:  
   A `NearestNeighbors` model is trained using cosine distance to measure similarity between songs.

3. **Recommendation Function**:  
   You input a song name, and it returns the most similar tracks based on audio characteristics.

---
