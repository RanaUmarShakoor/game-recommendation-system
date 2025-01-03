# Game Recommendation System 🎮

A Python-based recommendation system that suggests games similar to a given title using text-based feature extraction and cosine similarity.

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

The Game Recommendation System uses a content-based filtering approach to recommend games. It processes game metadata, extracts textual features, and calculates similarity scores to provide personalized suggestions.

---

## Features

- Content-based filtering using game metadata
- Text feature extraction with `CountVectorizer`
- Cosine similarity for game recommendations
- Memory-efficient processing with sparse matrices

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Scipy

---

## Dataset

The project uses the following datasets:
1. **Users Dataset** (`users.csv`): Contains user-related information.
2. **Games Dataset** (`games.csv`): Metadata about games, including tags and app IDs.
3. **Games Metadata** (`games_metadata.json`): Detailed information about games, such as genres, developers, and tags.

Ensure these datasets are placed in the `datasets` folder.

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

4. Place the required datasets in the `datasets` directory.

---

## Usage

1. Run the script:
    ```bash
    python game_recommendation.py
    ```

2. Modify the `game_to_recommend` variable in the `if __name__ == "__main__":` block to input a game title from the dataset.

3. View the recommendations in the console output.

---

## Example

### Input:
```python
game_to_recommend = "Escape Dead Island"
