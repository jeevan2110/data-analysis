# 🎬 Movie Dataset Analysis  

## 📌 Dataset Description  
This dataset contains information about **9,827 movies**, extracted from the **TMDB API**. It includes details such as release dates, genres, popularity, vote counts, ratings, and more.  

The dataset can be used for exploratory data analysis (EDA) to uncover insights into movie genres, audience preferences, and industry trends.  

---

## 📊 Columns Description  
- **Release_Date** → Date when the movie was released.  
- **Title** → Name of the movie.  
- **Overview** → Brief summary of the movie.  
- **Popularity** → Metric computed by TMDB developers based on number of views, votes per day, favorites, watchlist, and release timing.  
- **Vote_Count** → Total number of votes received.  
- **Vote_Average** → Average rating out of 10.  
- **Original_Language** → The original language of the movie (dubbed versions excluded).  
- **Genre** → Movie categories (comma-separated, e.g., Action, Drama).  
- **Poster_Url** → Link to the movie’s poster.  

---

## ❓ EDA Questions  
We focus on answering the following questions during analysis:  

1. **What is the most frequent genre in the dataset?**  
2. **Which genres received the highest votes?**  
3. **What movie has the highest popularity, and what is its genre?**  
4. **Which year had the most movies filmed?**  

---

## 🛠️ Data Wrangling  
- Dataset file: `mymoviedb.csv` (downloaded from Kaggle).  
- Rows & Columns: **9,827 rows × 9 columns**.  
- Initial checks showed no missing values or duplicates.  
- **Transformations applied:**  
  - `Release_Date` → Converted to datetime, extracted **Year**.  
  - Dropped irrelevant columns: `Overview`, `Original_Language`, `Poster_Url`.  
  - Outliers in `Popularity` handled.  
  - `Vote_Average` categorized for better grouping.  
  - `Genre` split into multiple rows (since movies can belong to multiple genres).  

After cleaning, the final dataset contained **25,551 rows × 6 columns**.  

---

## 📈 Data Visualization  
We used **Matplotlib** and **Seaborn** to generate meaningful charts and graphs.  

Key visuals include:  
- **Bar plots** for most frequent genres.  
- **Box plots** showing vote distribution across genres.  
- **Scatter plots** for popularity vs votes.  
- **Yearly trend plots** for number of movies released.  

---

## ✅ Conclusions  
**Q1: Most frequent genre?**  
- 🎭 **Drama** is the most frequent genre, appearing in **14% of movies** (out of 19 genres).  

**Q2: Genres with highest votes?**  
- Drama leads again, making up **18.5% of highly voted movies**.  

**Q3: Movie with highest popularity?**  
- 🕷️ *Spider-Man: No Way Home*  
- Genres: **Action, Adventure, Science Fiction**.  

**Q4: Year with most movies filmed?**  
- 📅 **2020** had the highest number of movie releases.  

---

## 📂 File Information  
- **Dataset File**: `mymoviedb.csv`  
- **Notebook**: `movie_analysis.ipynb` (contains cleaning, EDA, and visualizations)  
- **Language**: Python (Pandas, Matplotlib, Seaborn)  

---

✨ This project provides insights into movie industry trends, genre dominance, and audience preferences using real-world TMDB data.  
