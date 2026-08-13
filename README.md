# 🎬 IMDB Movie Analysis Project

An end-to-end IMDB Movie Data Analysis project using Python, Pandas, NumPy, MySQL, SQL, and Matplotlib/Seaborn.

The project covers data cleaning and preprocessing, duplicate handling, missing-value treatment, MySQL database storage, SQL analytics, Python-based analysis, and data visualization.

---

## 🎯 Project Objectives

- Clean and preprocess the raw IMDB movie dataset
- Handle missing values according to defined business rules
- Identify and remove duplicate movie records
- Apply business rules for duplicate movie selection
- Generate a unique `movie_id` for each movie
- Store the cleaned movie data in MySQL
- Perform analytical queries using SQL
- Retrieve SQL results into Pandas DataFrames
- Analyze movie ratings, genres, directors, budgets, and gross income
- Create visualizations using Matplotlib and Seaborn
- Identify meaningful insights from the analysis
- Provide conclusions and recommendations based on the analysis

---

## 🛠️ Technical Stack

| Technology | Purpose |
|------------|---------|
| Python | Data cleaning and analysis |
| Pandas | Data preprocessing and DataFrames |
| NumPy | Numerical operations |
| MySQL | Database storage and management |
| SQL | Data analysis and querying |
| mysql-connector-python | Python–MySQL connection |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Google Colab | Development environment |
| Git | Version control |
| GitHub | Project repository |

---

## 📊 Dataset

The project uses an IMDB movie dataset containing movie-related information such as:

- Movie title
- Genre
- Rating
- Budget
- Gross income
- Director
- Lead actor
- Release year
- Movie ID

The raw dataset contains **5,500 movie records and 9 columns**.

---

## 🧹 Data Cleaning and Preprocessing

The dataset was cleaned using defined business rules.

### BR-01: Duplicate Movie Handling

A movie is considered a duplicate when the following combination is repeated:

```text
title + release_year
