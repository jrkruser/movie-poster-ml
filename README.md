# Movie Poster ML

This repository contains a machine learning project focused on using movie poster images to predict movie revenue or other related factors. The project is currently a work in progress, and the dataset is being prepared and refined for analysis.

## Project Overview

The goal of this project is to explore whether features from movie posters can help predict movie success, particularly by predicting movie revenue. We will use a combination of metadata from movies (e.g., budget, genres, release date) and visual features extracted from the posters themselves.

## Dataset

### `movies.csv`
- This is a reduced version of the original Kaggle movie dataset, filtered for:
  - Movies with revenue greater than $100,000.
  - Movies with the original language set to English (`original_language = 'en'`).
- You can find the full dataset [here on Kaggle](https://www.kaggle.com/datasets/akshaypawar7/millions-of-movies/data).

### `posters/`
- This folder contains a sample of movie poster images used in this project. The full poster set is too large to host on GitHub, so we provide a sample of 100 images in the `posters/` folder. These are all jpeg images but require image processing and standardization.

### `omdb_enriched_data.csv`
- This CSV file contains the output of the `acquire_data.ipynb` and is the result of processing the Kaggle `movies.csv` dataset by enriching it with additional data from OMDb, such as poster URLs, ratings, and other metadata fields related to the movies. This data requires cleaning.

### `acquire_data.ipynb`
- This notebook contains the code used to fetch movie posters from OMDb and enrich the movie metadata with poster paths for further analysis.

## Structure

- **`movies.csv`**: A preprocessed CSV file with movie metadata.
- **`posters/`**: A sample folder of movie posters.
- **`omdb_enriched_data.csv`**: A CSV file containing the enriched movie data with OMDb metadata.
- **`acquire_data.ipynb`**: The notebook that fetches poster images and preprocesses the movie dataset.

## Getting Started

