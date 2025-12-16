# ECHOES - Spotify Recommendation System

ECHOES is a music recommendation system that combines graph-based collaborative filtering and machine learning techniques to provide personalized Spotify song recommendations. The system uses a hybrid approach with decision trees and graph-based user similarity to discover new music based on user preferences.

## Features

### **Dual Recommendation Engines**
- **Graph-based User Recommendations**: Uses collaborative filtering through a bipartite graph of users and songs to find similar users and recommend their favorite tracks
- **Decision Tree Song Analysis**: Employs machine learning to analyze audio features (acousticness, danceability, tempo, etc.) and recommend songs with similar characteristics

### **Spotify Integration**
- OAuth 2.0 authentication for secure Spotify account access
- Real-time access to user's listening history, playlists, and top tracks
- Integration with Spotify Web API for comprehensive music data

### **Modern GUI Interface**
- Built with CustomTkinter
- Tabbed navigation
- User-friendly login and recommendation display

### **Advanced Analytics**
- Decision tree visualization for understanding recommendation logic
- Audio feature analysis using cosine similarity
- Personalized recommendation scoring


## Tech Stack

- **Python 3.x** - Core programming language
- **Spotipy** - Spotify Web API wrapper
- **CustomTkinter** - Modern GUI framework
- **Pandas & NumPy** - Data manipulation and analysis
- **Scikit-learn** - Machine learning algorithms
- **Flask** - OAuth callback handling
- **Graphviz** - Decision tree visualization


## How It Works

### Graph-Based Recommendations
1. Creates a bipartite graph with user and song vertices
2. Establishes edges between users and their listened songs
3. Finds users with similar music taste
4. Recommends songs from similar users' libraries

### Decision Tree Recommendations
1. Analyzes audio features of songs (tempo, energy, valence, etc.)
2. Builds a decision tree based on user preferences
3. Uses the trained model to classify and recommend new songs
4. Applies cosine similarity for feature-based matching

### Authentication Flow
1. User initiates login through the GUI
2. Flask server handles OAuth callback from Spotify
3. Access tokens are securely stored and managed
4. User data is fetched and processed for recommendations

## Use Guide

1. **Launch the application** and click "Login with Spotify"
2. **Authenticate** your Spotify account through the browser
3. **Explore recommendations** in the user interface:
   - View graph-based recommendations from similar users
   - Discover songs through decision tree analysis
   - See detailed information about recommended tracks