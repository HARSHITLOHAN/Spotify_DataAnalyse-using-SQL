# 🎧 Spotify Data Analysis using SQL

Welcome to my **Spotify Data Analysis** project!  
This project showcases how SQL can be used to explore and analyze a music dataset, uncover hidden trends, and solve real-world business problems using powerful SQL techniques.

> 🚀 **About Me:** I'm a Computer Science student learning Data Analytics by building real projects. I already knew SQL but now I’m applying it to analyze datasets and develop real insights. This hands-on approach is speeding up my learning!

---

## 📌 Project Objective

This project focuses on:

- Understanding the structure of a large Spotify dataset  
- Cleaning and preparing the data for analysis  
- Solving music industry-related business problems  
- Using **advanced SQL** to extract useful insights

---

## 🗃️ Dataset Structure

The dataset is stored in a table called `spotify`. It contains **21 columns**, covering track metadata, audio features, performance metrics, and user engagement data.

| Column Name       | Data Type     | Description |
|-------------------|---------------|-------------|
| artist            | VARCHAR       | Name of the artist |
| track             | VARCHAR       | Track name |
| album             | VARCHAR       | Album name |
| album_type        | VARCHAR       | Type of album (single/album) |
| danceability      | FLOAT         | Dance suitability (0.0 to 1.0) |
| energy            | FLOAT         | Intensity and activity |
| loudness          | FLOAT         | Loudness in dB |
| speechiness       | FLOAT         | Spoken word presence |
| acousticness      | FLOAT         | Acoustic confidence |
| instrumentalness  | FLOAT         | Instrumental confidence |
| liveness          | FLOAT         | Live performance probability |
| valence           | FLOAT         | Musical positivity |
| tempo             | FLOAT         | Beats per minute |
| duration_min      | FLOAT         | Track length in minutes |
| title             | VARCHAR       | Content title |
| channel           | VARCHAR       | Channel name |
| views             | FLOAT         | YouTube views |
| likes             | BIGINT        | Likes on content |
| comments          | BIGINT        | Total comments |
| licensed          | BOOLEAN       | Is content licensed? |
| official_video    | BOOLEAN       | Has official video? |
| stream            | BIGINT        | Spotify streams |
| energy_liveness   | FLOAT         | Ratio of energy to liveness |
| most_played_on    | VARCHAR       | Platform with most plays |

---

## 📊 Exploratory Data Analysis (EDA)

Steps taken during EDA:

- Counted total and unique records in key columns like `artist`, `track`, `album`
- Calculated **min/max** for features such as `energy` and `duration_min`
- Removed invalid data (e.g., tracks with `duration_min = 0`)
- Identified distribution ranges for audio features

---

## 📈 Business Problems Solved

Here are the key questions solved using SQL:

1. 🎵 **Popular Tracks:** Tracks with over 1 billion streams
2. 📀 **Album Insights:** Albums with their artists
3. 💬 **Engagement:** Total comments on licensed content
4. 🎶 **Single Type Tracks:** Tracks marked as “single”
5. 🧑‍🎤 **Artist Productivity:** Total tracks per artist
6. 💃 **Danceability:** Average danceability per album
7. 🔋 **Top Energy Tracks:** 5 tracks with highest energy
8. 📺 **Official Video Metrics:** Views and likes on official videos
9. 👑 **Album Performance:** Total views per album
10. 🔁 **Spotify vs YouTube:** Tracks streamed more on Spotify than YouTube
11. 🎯 **Top Tracks by Artist:** Top 3 most-viewed tracks per artist (Window Functions)
12. 🔊 **Liveness:** Tracks with above-average liveness
13. ⚡ **Energy Range:** Max - Min energy per album (using CTE)
14. 📊 **Energy/Liveness Ratio:** Tracks where energy/liveness > 1.2
15. 💓 **Cumulative Likes:** Likes sorted by views (using Window Functions)

---

## 🧠 SQL Techniques Used

| Technique             | Description |
|-----------------------|-------------|
| ✅ Basic Queries       | `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`, `LIMIT` |
| ✅ Aggregations        | `COUNT`, `SUM`, `AVG`, `MIN`, `MAX` |
| ✅ Subqueries          | For comparison metrics (e.g., above-average liveness) |
| ✅ Window Functions    | `DENSE_RANK`, `SUM() OVER()` for ranking and running totals |
| ✅ CTEs (WITH Clause)  | For breaking down complex logic into readable parts |

---

## ⚙️ How to Run the Project

1. Clone this repository.
2. Load the dataset into your SQL environment (MySQL/PostgreSQL/BigQuery/etc.).
3. Use the `CREATE TABLE` query to set up the schema.
4. Insert the dataset into the `spotify` table.
5. Run the provided SQL queries one by one to see the results.

---

## 🌟 Key Insights

- **Artist Dominance:** Some artists are far more productive, releasing the majority of the platform's top content.
- **Track Popularity:** Higher energy, valence, and danceability often correlate with more streams and views.
- **Video Engagement:** Tracks with official videos and proper licensing tend to receive more user interaction.
- **Platform Preference:** Some tracks perform better on Spotify, others dominate YouTube—this can help tailor marketing strategies.

---

## 🎯 Project Goals

This project was built to:

- 📊 Strengthen my SQL skills with real-world data
- 🧠 Develop business thinking using analytical techniques
- 🔍 Learn how to clean, explore, and interpret large datasets
- 🧑‍💻 Transition from basic SQL knowledge to actual **Data Analytics**

---

> 🧘‍♂️ *Learning by doing makes knowledge stick. This project helped me move from theory to practice — and that's the real win for me as a Data Analyst in the making.*

---

**Made with 💻 and 🎵 by a CSE student learning Data Analytics**  
📩 Feel free to connect if you want to collaborate or ask questions!

