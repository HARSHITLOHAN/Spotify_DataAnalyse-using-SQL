🎧 Spotify Data Analysis Using SQL
🔍 Project Overview
This project explores a real-world Spotify dataset using SQL to extract insights about music trends, artist performance, and listener behavior. It focuses on data exploration, cleaning, and analysis, leveraging advanced SQL techniques like window functions, aggregations, and CTEs.

✅ As a Computer Science student with prior SQL knowledge, this project is helping me apply that foundation to learn Data Analytics practically and effectively.

📚 Table of Contents
Data Structure

Exploratory Data Analysis (EDA)

Business Problems Analyzed

SQL Techniques Used

How to Run the Project

Goals & Explanation

Key Features

Key Insights

🧱 Data Structure
The dataset is stored in a SQL table called spotify with the following schema:

Column Name	Data Type	Description
artist	VARCHAR(255)	Artist name
track	VARCHAR(255)	Track name
album	VARCHAR(255)	Album name
album_type	VARCHAR(50)	Type of album (e.g., single, album)
danceability	FLOAT	Suitability for dancing (0.0–1.0)
energy	FLOAT	Intensity and activity level
loudness	FLOAT	Loudness in dB
speechiness	FLOAT	Spoken word presence
acousticness	FLOAT	Acoustic confidence
instrumentalness	FLOAT	Instrumental confidence
liveness	FLOAT	Live performance likelihood
valence	FLOAT	Musical positivity
tempo	FLOAT	Tempo in BPM
duration_min	FLOAT	Duration in minutes
title	VARCHAR(255)	Content title
channel	VARCHAR(255)	Channel name
views	FLOAT	Total views
likes	BIGINT	Total likes
comments	BIGINT	Total comments
licensed	BOOLEAN	Licensed (TRUE/FALSE)
official_video	BOOLEAN	Has official video (TRUE/FALSE)
stream	BIGINT	Total streams
energy_liveness	FLOAT	energy ÷ liveness
most_played_on	VARCHAR(50)	Platform with most plays (Spotify/YouTube)

📊 Exploratory Data Analysis (EDA)
Initial analysis steps included:

Counting total and unique records in key columns (artist, track, album, etc.)

Checking min and max for features like energy and duration_min

Removing invalid rows (duration_min = 0)

Understanding distributions for audio features

💼 Business Problems Analyzed
This project tackled practical business questions using SQL:

Track Popularity: Tracks with more than 1 billion streams

Album Insights: All albums with corresponding artists

Engagement Metrics: Total comments on licensed tracks

Album Type Filter: Tracks labeled as “single”

Artist Productivity: Total tracks by each artist

Danceability Trends: Average danceability per album

Top Energy Tracks: Top 5 tracks with highest energy

Official Video Performance: Views & likes for official videos

Album Performance: Total views per album

Platform Preference: Tracks streamed more on Spotify than YouTube

Top Tracks by Artist: Top 3 most-viewed tracks per artist

Liveness Analysis: Tracks with above-average liveness

Energy Range: Energy range per album (using CTE)

Energy-Liveness Ratio: Tracks where energy / liveness > 1.2

Cumulative Likes: Using window functions on likes ordered by views

🛠️ SQL Techniques Used
Basic Queries: SELECT, WHERE, GROUP BY, ORDER BY, LIMIT

Aggregations: COUNT, SUM, AVG, MIN, MAX

Window Functions: DENSE_RANK, SUM OVER, etc.

CTEs (Common Table Expressions): Simplify multi-step logic

Subqueries: For comparisons (e.g., above-average liveness)

⚙️ How to Run the Project
Load the dataset into your SQL environment.

Run the CREATE TABLE query based on the schema.

Insert the data into the spotify table.

Run the queries (in order) to perform the analysis and see insights.

🎯 Goals & Explanation
This project helped me transition from knowing SQL as a CSE student to using it for data-driven storytelling. It focuses on:

🧹 Data Exploration: Understand and clean the dataset

💡 Business Insights: Solve real-world music streaming problems

🧠 SQL Mastery: Apply advanced SQL to meaningful problems

✨ Key Features
🎵 1. Rich Dataset
Covers tracks, albums, artists, platforms

Includes performance metrics: views, likes, streams, etc.

Audio features: energy, tempo, danceability, liveness, etc.

🧽 2. Data Cleaning & EDA
Removed anomalies like zero-duration tracks

Profiled artists and albums

Explored audio and performance trends

📈 3. Real-World Problem Solving
Artist-wise productivity

Platform performance comparison

Engagement insights for videos and licensed content

Track rankings using advanced SQL

🧠 4. Advanced SQL
CTEs and subqueries to keep logic clean

Window functions for ranking and cumulative metrics

Aggregate functions to extract trends

📌 Key Insights
🎤 Artist Dominance: Track count reveals artist productivity

🔥 Track Popularity: High energy and danceability correlate with top-streamed tracks

🎥 Official Content Wins: Videos and licensed tracks drive more engagement

📱 Platform Preference: Some tracks perform better on Spotify, others on YouTube

🙌 Learning Note:
As someone moving from CSE foundations to Data Analytics, this project made SQL feel powerful. It’s helping me build confidence by applying real techniques to real data. It’s not just learning — it’s doing.

