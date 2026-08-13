# 🎬 IMDB Movie Analysis Project

An end-to-end IMDB movie data analysis project that demonstrates data cleaning, validation, duplicate handling, SQL database management, Python data analysis, Matplotlib visualization, and analytical reporting.

---

## 📌 Project Overview

This project analyzes IMDB movie data containing information such as movie titles, release years, ratings, genres, directors, actors, budgets, and gross income.

The project follows an end-to-end data pipeline:

Raw CSV Data  
↓  
Data Profiling  
↓  
Data Cleaning  
↓  
Data Validation  
↓  
MySQL Database  
↓  
SQL Analysis  
↓  
Python + Pandas  
↓  
Matplotlib Visualization  
↓  
Key Findings & Recommendations

---

## 🎯 Objectives

- Clean and preprocess the raw IMDB movie dataset
- Identify and handle missing values
- Identify and remove duplicate movie records
- Apply defined business rules for duplicate handling
- Store cleaned data in MySQL
- Perform analytical queries using SQL
- Retrieve and analyze data using Python and Pandas
- Create visualizations using Matplotlib
- Identify key findings from the analysis
- Provide recommendations based on the analysis

---

## 🛠️ Technical Stack

| Technology | Purpose |
|------------|---------|
| Python | Data processing and analysis |
| Pandas | Data cleaning and DataFrames |
| NumPy | Numerical operations |
| MySQL | Structured data storage |
| SQL | Data analysis and querying |
| mysql-connector-python | Python-MySQL connection |
| Matplotlib | Data visualization |
| Google Colab | Development environment |
| Git | Version control |
| GitHub | Repository hosting |

---

## 📂 Project Structure

IMDB-MOVIE-ANALYSIS/
│
├── data/
│   ├── raw/
│   │   └── imdb_movies.csv
│   └── cleaned/
│       └── cleaned_imdb_movies.csv
│
├── sql/
│   └── analysis_queries.sql
│
├── notebooks/
│   └── IMDB_Movie_Analysis.ipynb
│
├── visualizations/
│   ├── rating_distribution.png
│   ├── genre_analysis.png
│   └── top_grossing_movies.png
│
├── README.md
├── requirements.txt
└── .gitignore

---

## 🧹 Data Cleaning

The dataset was cleaned using defined business rules.

### Duplicate Handling

A movie is considered a duplicate when:

- `title`
- `release_year`

are repeated.

The duplicate record with the **highest rating** is retained.

If ratings are equal, the record with the **highest gross** is retained.

---

## 🔍 Data Analysis

The project performs analysis such as:

- Top-rated movies
- Top-grossing movies
- Movie ratings distribution
- Genre-wise analysis
- Year-wise movie trends
- Director performance
- Gross income analysis
- Movie budget analysis

---

## 📊 Data Visualization

Matplotlib is used to create visualizations for:

- Rating distribution
- Top-grossing movies
- Genre performance
- Year-wise trends
- Other analytical findings

---

## 🗄️ MySQL Analysis

The cleaned dataset is loaded into MySQL and SQL queries are used to perform analytical operations such as:

- Aggregations
- Filtering
- Sorting
- GROUP BY analysis
- JOIN operations
- Ranking
- Top-N analysis

---

## 📈 Key Findings

The analysis identifies important patterns in:

- Movie ratings
- Gross income
- Movie genres
- Release years
- Directors
- Movie performance

---

## 💡 Recommendations

Based on the analysis, recommendations are provided regarding:

- High-performing movie genres
- Rating and audience preferences
- Revenue-generating movies
- Trends across release years
- Factors associated with movie performance

---

## 🏁 Conclusion

This project demonstrates an end-to-end data analytics workflow using **Python, Pandas, NumPy, MySQL, SQL, and Matplotlib**.

It covers the complete process from raw data cleaning and validation to database management, SQL analysis, visualization, and business insights.

---

## 👨‍💻 Author

**Rakesh Akurathi**
