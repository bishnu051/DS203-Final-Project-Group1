# 📄 README – MUBI Platform Movie List and Rating Analysis using PySpark

## 📚 Project Description

This project analyzes user behavior on the **MUBI** streaming platform using **PySpark**.  
MUBI is a curated streaming service specializing in art-house, international, and independent cinema.  
We explore how users interact with movie **lists** and **ratings** to understand movie popularity and user curation trends.

The datasets were sourced from Kaggle:  
🔗 [MUBI SQLite Database for Movie Lovers](https://www.kaggle.com/datasets/clementmsika/mubi-sqlite-database-for-movie-lovers?select=mubi_ratings_user_data.csv)

## 🗂️ Datasets Used
- `mubi_lists_data.csv` — movie entries per user-created list
- `mubi_lists_user_data.csv` — list-level user metadata
- `mubi_movie_data.csv` — movie information (titles, directors, etc.)
- `mubi_ratings_data.csv` — overall movie ratings
- `mubi_ratings_user_data.csv` — user-specific movie ratings

## 🔍 Analysis Performed

### 1. Most Followed Lists
- Extracted the top 10 lists with the highest follower counts.
- Cleaned the data to remove nulls and duplicates.
- Sorted based on `list_followers` after type casting.

### 2. Movies Most Frequently Appearing in Top Lists
- Selected the top 100 most followed lists.
- Retrieved all movies included in those lists.
- Identified which movies appeared most frequently across the most popular lists.

## ⚙️ Tools and Technologies
- **PySpark** — for distributed data processing
- **Google Colab** — for running PySpark notebooks easily
- **Kaggle** — for sourcing datasets

## 📈 Key Results
- Most popular lists focus on curated themes like "100 Greatest Films" and "Best Films by Year."
- Top movies frequently included in popular lists are international cinema titles and classic masterpieces.
- MUBI users tend to favor curated discovery and thematic exploration over random browsing.

## 🚀 How to Reproduce
1. Upload the Kaggle MUBI CSV files into Google Colab.
2. Run the PySpark environment setup.
3. Clean datasets (drop duplicates, cast types).
4. Perform joins and aggregations as shown in the notebook.
5. Generate insights on most popular lists and most included movies.

## 📎 References
- [MUBI Official Website](https://mubi.com/)
- [MUBI Dataset on Kaggle](https://www.kaggle.com/datasets/clementmsika/mubi-sqlite-database-for-movie-lovers)
- [PySpark Documentation](https://spark.apache.org/docs/latest/api/python/index.html)
