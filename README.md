# Music recommendation system using spotify dataset

## Overview
This repository contains a music recommendation system built using the Spotify dataset. The system employs various data analysis and machine learning techniques to recommend songs based on user preferences, utilizing libraries such as Pandas, NumPy, Seaborn, Plotly, and Scikit-learn.

## Features
- **Data Visualization**: Visualize audio features and popularity trends over decades.
- **Clustering**: Group songs into clusters using KMeans for better recommendations.
- **Dimensionality Reduction**: Use PCA and t-SNE for visualizing high-dimensional data.
- **Recommendation Engine**: Recommend songs based on the user's listening history using Spotipy.

## Requirements
To run this project, you need:
- Python 3.x
- Libraries:
  - Pandas
  - NumPy
  - Seaborn
  - Plotly
  - Matplotlib
  - Scikit-learn
  - Spotipy
- Install the required libraries using pip:
```bash
pip install pandas numpy seaborn plotly matplotlib scikit-learn spotipy yellowbrick
```

## Getting Started

### Dataset
The dataset used in this project can be found in the repository. It includes various audio features of songs from Spotify.

### Setup Spotipy
1. Create an app on the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).
2. Obtain your Client ID and Client Secret.
3. Store your credentials in environment variables or directly in the code (not recommended for production).

### Running the Code
1. Clone the repository:
```bash
git clone https://github.com/yourusername/music-recommendation-system-using-spotify-dataset.git
cd music-recommendation-system-using-spotify-dataset
```
2. Open a Jupyter Notebook or any Python environment.
3. Import necessary libraries and load the dataset:
```python
import pandas as pd

data = pd.read_csv('path_to_your_dataset.csv')
```
4. Execute the provided code to visualize data, cluster songs, and make recommendations.

## Code Explanation

### Data Visualization
The code includes functions to visualize audio features and their correlations with popularity using Seaborn and Plotly.

### Clustering Songs
Using KMeans clustering, songs are grouped based on their audio features to identify similar tracks.

### Recommendation System Logic
The recommendation system calculates distances between songs in a multi-dimensional space to suggest tracks that are similar to those already liked by the user.

### Example of Finding Recommendations:
```python
recommend_songs([{'name': 'Song name from dataset', 'year':Year of song from dataset}], data)
```


## License
This project is licensed under the MIT License. See the LICENSE file for more details.

