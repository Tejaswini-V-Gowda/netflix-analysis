# 📺 Netflix Titles Dataset – Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project explores the **Netflix Titles Dataset** (from Kaggle), which contains ~8,800 rows of metadata about Movies and TV Shows available on Netflix.  
The main goal of this analysis is to understand **viewing trends, content types, and popular countries** using data cleaning, feature engineering, and visualization.  

---

## 📊 Dataset Information
- **Rows:** 8,807  
- **Columns:** 12  
- **Key Columns:**  
  - `type` → Movie or TV Show  
  - `title` → Title of the content  
  - `director`, `cast` → People involved  
  - `country` → Country of production  
  - `date_added` → When it was added to Netflix  
  - `release_year` → Original release year  
  - `rating` → Content rating (e.g., PG, TV-MA)  
  - `duration` → Duration in minutes (movies) or number of seasons (TV shows)  
  - `listed_in` → Genre(s)  
  - `description` → Short description  

---

## 🛠 Steps Performed
1. **Data Understanding & Cleaning**
   - Converted `date_added` to datetime format.  
   - Handled missing values (`director`, `cast`, `country`, `rating`, `duration`).  
   - Created new features:  
     - `release_decade` (e.g., 1990s, 2000s, 2010s)  
     - `is_movie` (1 = Movie, 0 = TV Show).  

2. **Feature Engineering**
   - Extracted year-based trends from `release_year`.  
   - Grouped countries into **Top 5** + "Other".  

3. **EDA & Visualization**
   - Pie chart of **Movies vs TV Shows**.  
   - Line plot of content released per year.  
   - Barplot of **Top 10 genres**.  
   - Heatmap of **Country vs Content Volume**.  

---

## 🔑 Key Insights
- **Content Type Distribution:** ~69.6% Movies, ~30.4% TV Shows.  
- **Top Content-Producing Countries:**  
  1. United States  
  2. India  
  3. United Kingdom  
  4. Japan  
  5. South Korea  
- **Genres:** Dramas, Documentaries, and Comedies dominate Netflix’s library.  
- **Yearly Trend:** Sharp growth in Netflix content after 2015, reflecting global expansion.  

---

## ▶️ How to Run
1. Clone the repository:  
   ```bash
   git clone https://github.com/Tejaswini-V-Gowda/netflix-analysis.git
   cd netflix-analysis
