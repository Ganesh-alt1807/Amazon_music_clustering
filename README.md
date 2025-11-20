Amazon Music Clustering – Unsupervised Learning Project
📌 Overview

This project uses unsupervised machine learning to group Amazon Music tracks into clusters based on their audio characteristics.
The goal is to identify natural song groups (e.g., acoustic, energetic, instrumental, chill) without using genre labels.

🎯 Objectives

Perform data cleaning and preprocessing

Select musical audio features

Normalize the dataset

Choose optimal number of clusters

Apply KMeans clustering

Visualize clusters using PCA

Interpret musical characteristics of each cluster

Export final clustered dataset

📂 Dataset

Contains audio features describing each track:

danceability  
energy  
loudness  
speechiness  
acousticness  
instrumentalness  
liveness  
valence  
tempo  
duration_ms  


Optional metadata (based on availability):

track_id  
track_name  
artist_name

🧹 Preprocessing

Removed unnecessary text metadata from clustering input

Handled missing values

Standardized features using StandardScaler

Conducted EDA (distribution plots, correlation heatmap)

🔍 Choosing the Best k

Used a fast & efficient approach:

PCA (5 components) for faster search

MiniBatchKMeans for rough testing

Silhouette score for accuracy

Refined search around best k

Final chosen:

k = YOUR_K_HERE

🤖 Final Model

Algorithm: KMeans

n_init: 20

Input: full scaled dataset

Output: cluster label added to dataset

📊 Visualizations

PCA 2D cluster scatter plot

Cluster profile table (mean feature values per cluster)

📤 Output Files
amazon_music_clusters_final.csv
representative_tracks_by_cluster.csv


These include cluster assignments and PCA components.

🚀 How to Run

Open the Jupyter Notebook

Run all cells sequentially

Final CSV and results will be saved automatically

📘 Conclusion

This project demonstrates how unsupervised learning can reveal hidden structure in music data.
The clusters provide valuable insights for:

Playlist generation

Music discovery

Artist similarity

Recommendation systems

Market analysis

⭐ Author

Ganesh
