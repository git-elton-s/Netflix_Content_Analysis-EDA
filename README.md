# 🍿 Netflix Content Analysis: Comprehensive EDA

This project performs a comprehensive exploratory data analysis (EDA) of the Netflix Movies and TV Shows dataset from Kaggle The project was developed entirely in Google Colab.
The goal is to understand how Netflix builds its catalog by examining trends in content types, genres, ratings, geography, release patterns, and textual descriptions.

- [Google Colab Notebook](https://colab.research.google.com/drive/17g3uR3aDsvkD7TdmmwqFyxDgOb23vfEc?usp=sharing)
- [Dataset Source](https://github.com/git-elton-s/Datasets/tree/main/Netflix_Titles_Dataset)

## 📊 What This Project Covers
### 1. Data Loading & Cleaning
- Inspection of dataset structure and missing values
- Imputation and cleaning of key fields (director, cast, country, rating)
- Conversion of date fields and extraction of year_added and month_added
- Handling of multi-valued columns using explode techniques

### 2. Feature Engineering
Additional features were created to support richer analysis:
- `year_added` and `month_added`
- `age_on_netflix` (gap between release year and Netflix addition)
- Expanded genre, country, and cast lists
- Cleaned rating categories for clearer time-series analysis

### 3. Visualization & Analysis
A wide range of visual techniques were used:
- Content type distributions (Movies vs TV Shows)
- Time-series trends of how content was added over the years
- Genre, country, and rating breakdowns
- Duration analysis for Films and TV Shows
- Heatmaps comparing release year vs year added
- NLP visualizations including WordClouds, bigram and trigram frequency plots

### 4. Key Insights
- Netflix’s catalog is movie-heavy, with ~70% of titles being films.
- A major expansion occurred between 2016–2019, driven by both Originals and older licensed content.
- The US and India are the largest content contributors.
- Mature ratings (TV-MA, TV-14) dominate the platform’s additions.
- Most TV Shows have only one season, while movies typically run 80–120 minutes.
- Descriptions frequently reference young characters, real-life events, and familiar settings like New York and small towns.

### 5. NLP Analysis
- Using NLTK and Scikit-Learn:
- Extracted most common word pairs (bigrams)
- Extracted most frequent three-word phrases (trigrams)
- Revealed recurring themes such as coming-of-age stories, true events, personal journeys, and dramatic transformation

This repository offers a complete reference for understanding the structure, themes, and evolution of Netflix’s catalog. It provides a strong foundation for further machine learning tasks such as content recommendation, clustering, or predictive modeling.
