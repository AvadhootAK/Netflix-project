

# 🎬 Movie Data Analysis Project

This project presents an in-depth exploratory data analysis (EDA) of a curated movie dataset. The primary goal is to uncover patterns related to movie popularity, voting trends, genres, and release patterns over time. Using Python and Jupyter Notebook, the analysis transforms raw data into meaningful insights for film fans, analysts, and content curators.

---

## 📚 Project Overview

The dataset contains metadata about various movies including:

* Title, Genre, Language
* Popularity score
* Vote count and average rating
* Release date

The analysis includes steps for data cleaning, transformation, categorization, and visualization. It answers key questions like:

* What genres are most commonly produced?
* How does voting behavior vary across movies?
* Are certain years more prolific or better rated than others?
* What’s the relationship between vote count and popularity?

---

## 🔧 Dataset Summary

The dataset (`mymoviedb.csv`) includes the following columns:

* `Title` – Movie name
* `Genre` – Primary and secondary genres (exploded for clarity)
* `Vote_Count` – Number of user votes
* `Vote_Average` – Average rating (scale of 0–10)
* `Popularity` – Platform-defined popularity metric
* `Release_Date` – Converted to year for temporal analysis
* Additional metadata such as `Overview`, `Poster_URL`, etc. (dropped for brevity)

---

## 🧹 Data Cleaning & Transformation

The notebook follows a structured data preparation workflow:

* Removed duplicate records
* Converted `Vote_Count` and `Vote_Average` to numeric values
* Dropped rows with missing essential data
* Parsed `Release_Date` into year-only values
* Exploded `Genre` into multiple rows to enable genre-level aggregation
* Bucketed vote averages into categorical popularity segments:

  * `not_popular`, `below_average`, `average`, `popular`

---

## 📊 Analysis Highlights

Some key analytical steps include:

* Genre frequency distribution
* Vote and popularity comparisons
* Trend analysis over time based on `Release_Date`
* Classification of movies by popularity level using quartile-based binning
* Dealing with multi-label genre fields using `explode`

Visualizations use `matplotlib` and `seaborn` to convey patterns in vote behavior, genre popularity, and more.

---

## 📈 Insights & Observations

* Movies are distributed unevenly across genres, with some dominating the dataset.
* There is a strong correlation between high vote counts and high popularity.
* The number of movies released fluctuates across years, with spikes during certain decades.
* Some genres consistently receive higher average votes than others.

---

## 🧰 Tools & Technologies

* `pandas` – data loading and cleaning
* `numpy` – numeric operations
* `matplotlib` – visualization
* `seaborn` – enhanced statistical plotting
* `Jupyter Notebook` – interactive, step-by-step exploration

---

## ✅ Use Cases

This notebook is an excellent foundation for:

* Academic EDA projects
* Building recommendation systems
* Movie popularity prediction models
* Content strategy planning in streaming platforms
* Learning data wrangling techniques on complex, multi-value fields (like genres)

---

## 🙌 Contributions & Feedback

Feel free to fork, extend, or modify this project to analyze your own movie datasets. Feedback, issues, and PRs are always welcome to improve the scope of the analysis.


