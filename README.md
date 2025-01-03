# Game Recommendation System 🎮

A Jupyter Notebook-based recommendation system that suggests games similar to a given title using text-based feature extraction and cosine similarity.

---

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Example](#example)

---

## Introduction

This project builds a Game Recommendation System using a content-based filtering approach. It leverages game metadata such as tags and genres to recommend games similar to a given game using text-based feature extraction and cosine similarity.

---

## Features

- Content-based filtering using game metadata (tags and genres)
- Text feature extraction with `CountVectorizer`
- Cosine similarity for game recommendations
- Memory-efficient processing using sparse matrices

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Scipy
- Jupyter Notebook

---

## Dataset

The project uses the following dataset:

- **Game Recommendations on Steam**: [Kaggle Dataset Link](https://www.kaggle.com/datasets/antonkozyriev/game-recommendations-on-steam)  
  This dataset includes metadata about Steam games, such as game titles, app IDs, tags, and other relevant details.

To use this dataset:
1. Download the dataset from Kaggle.
2. Place the relevant files (`games.csv`, `games_metadata.json`, etc.) in the `datasets` folder of the project.

---

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/game-recommendation-system.git
    cd game-recommendation-system
    ```

2. Create a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Download the dataset from Kaggle and place the files in the `datasets` folder.

---

## Usage

1. Open the Jupyter Notebook file (`Game_Recommendation_System.ipynb`).
2. Run all cells to load and preprocess the data, followed by generating game recommendations.
3. Modify the `game_to_recommend` variable to input a game title from the dataset.

---

## Example

### Input:
```python
game_to_recommend = "Escape Dead Island"
```

### Output:
```
Games similar to 'Escape Dead Island':
1. Sniper Elite: Nazi Zombie Army
2. How To Survive: Third Person Standalone
3. Cold Fear™
4. Sniper Elite: Nazi Zombie Army 2
5. The Evil Within 2
```
