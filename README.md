# Anime Recommendation System using Graph Neural Networks

This repository contains an **anime recommendation system** built using **Graph Neural Networks (GNNs)**.
The model constructs a **graph from user-anime interactions and anime metadata(genres)**, with edges weighted by user ratings, to generate personalized recommendations.
It utilizes **Graph Attention Networks (GAT)** for learning meaningful embeddings.

## Features
- **Hybrid Recommendation System**: Combines **collaborative filtering** (user-item interactions) and **content-based filtering** (anime genres).
- **Graph-Based Approach**: Represents users and anime as a graph, where edges represent **ratings and anime similarity**.
- **Graph Attention Network (GAT)**: Learns **user and anime embeddings** by considering **edge weights (ratings)** for better recommendations.
- **Efficient Training with PyTorch Geometric**: Uses GNN-based learning for scalability.

---

## Dataset
This system is built using the **Anime Recommendations Database**:  

### **Anime.csv**
- `anime_id`: Unique anime ID.
- `name`: Anime title.
- `genre`: Comma-separated genres.
- `type`: TV, movie, OVA, etc.
- `episodes`: Number of episodes.
- `rating`: Average rating.
- `members`: Number of members who added this anime to their list.

### **Rating.csv**
- `user_id`: Unique user ID.
- `anime_id`: Anime rated by the user.
- `rating`: **User-assigned rating** (ranging from 1 to 10, or -1 if watched but not rated).

---
