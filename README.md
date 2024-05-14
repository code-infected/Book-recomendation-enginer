# Book Recommendation Algorithm using K-Nearest Neighbors

This project aims to develop a book recommendation algorithm using K-Nearest Neighbors (KNN) and the Book-Crossings dataset. KNN is a simple yet powerful algorithm for classification and regression tasks.

## Project Overview

In this challenge, we utilize the Book-Crossings dataset, which contains 1.1 million ratings (on a scale of 1-10) of 270,000 books by 90,000 users. The goal is to build a model that recommends books similar to a given book title.

## Getting Started

To get started, make sure you have the required libraries installed. You can install them using pip:

```bash
pip install numpy pandas scipy scikit-learn matplotlib
```

Additionally, you need to download the dataset. The required files are:

- [BX-Books.csv](https://cdn.freecodecamp.org/project-data/books/BX-Books.csv)
- [BX-Book-Ratings.csv](https://cdn.freecodecamp.org/project-data/books/BX-Book-Ratings.csv)

## Implementation

The implementation consists of the following steps:

1. Importing necessary libraries and data files.
2. Data cleaning: Removing users with less than 200 ratings and books with less than 100 ratings.
3. Using NearestNeighbors from scikit-learn to build the recommendation model.
4. Creating a function `get_recommends` that takes a book title as input and returns a list of 5 similar books along with their distances from the input book.
5. Testing the implementation with sample inputs.

## File Structure

```
- README.md               # This file
- book_recommendation.ipynb   # Jupyter Notebook containing implementation code
- BX-Books.csv            # Dataset: Book information
- BX-Book-Ratings.csv     # Dataset: Book ratings by users
```

## Usage

To use the recommendation system, simply call the `get_recommends` function with the title of the book you want recommendations for. For example:

```python
get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")
```

This will return a list of 5 similar books along with their distances from the input book.

## Dataset

The Book-Crossings dataset is used in this project, consisting of book ratings by users. It has been preprocessed to ensure statistical significance by removing users with less than 200 ratings and books with less than 100 ratings.

## Credits

This project is part of a challenge and utilizes resources provided by FreeCodeCamp.

