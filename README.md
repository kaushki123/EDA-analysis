 📊 EDA-analysis

This project presents an **Exploratory Data Analysis (EDA)** on a Netflix dataset. The analysis focuses on understanding the structure, trends, and insights from Netflix's catalog of shows and movies.

---

## 📁 Files Included

- [`netflix_titles.csv`](./netflix_titles.csv): Dataset containing Netflix content details such as title, type, director, cast, country, release year, rating, and genre.
- [`EXPLORATORY DATA ANALYSIS (Project ).ipynb`](./EXPLORATORY%20DATA%20ANALYSIS%20(Project%20).ipynb): Jupyter Notebook with step-by-step analysis and visualizations.

---

## 📌 Objectives:-

- Analyze the distribution of Movies vs. TV Shows.
- Explore top contributing countries, genres, and release years.
- Visualize missing values and data quality issues.
- Examine ratings and trends over time.

---

## 🛠️ Tools Used:-

- Python
- Pandas
- Matplotlib
- Seaborn

---

## ✅Key Insights from Netflix EDA Project :-
📁 Missing values are present primarily in:
* director
* cast
* country
These columns were cleaned and explored further to identify patterns (e.g., documentaries often lack cast or director info).

*  Date fields (date_added) were converted and split into:-
   * year_added
   * month_added
to allow temporal analysis.

🎬 Content Type Distribution:-
   * Movies make up approximately 70% of the content.
   *  TV Shows account for the remaining 30%, showing Netflix's stronger focus on movies.

🌍 Country Contribution:-
   * The United States is the top content provider on Netflix, followed by:
   * India
   * United Kingdom
   * Canada
* Several countries like South Korea, France, and Japan also show strong representation, especially in TV content.

🕰️ Temporal Trends:-
* Content additions increased significantly from 2017 onward, peaking in 2019 and 2020.
* This aligns with Netflix's global expansion and content push during the pandemic.
* Most added content comes in the months July to October, indicating seasonal acquisition trends.

🕹️ Ratings and Audience Categories:-
*  Extracting rating_grade from the rating column to group similar audience classifications.
* The most common content ratings are:
   * TV-MA, TV-14, PG-13, R
* A custom rating_grade column was created to assign letter grades (e.g., A, B, C, D) to ratings.
* The rating_description column adds clarity by mapping  rating, converting letter grades (like C+, D-) into human-readable descriptions  like:
  * “Adults only (mature content)”
  * “Teens, parental caution”
* Splitting the date_added column into year_added and month_added to analyze content trends over time more effectively.

📊 Duration Patterns:-
* Movies:
  * Duration mostly falls between 80–120 minutes.
* TV Shows:
   * Majority have 1–2 seasons, showing a trend toward short, bingeable series

 🎭 Genre & Categories:-
* Top genres include:
  * Dramas
  * Comedies
  * Documentaries
  * International Movies
* Many titles belong to multiple genres (e.g., “Dramas, International Movies”), so genre-based analysis used string splitting and grouping.


📈 Summary:-

- The majority of content on Netflix is Movies.
- Most content originates from the United States and India.
- A significant number of shows were added between 2018 and 2020.
- A majority of content is targeted at teen and adult audiences.

---

## 📌 How to Run:-

1. Clone the repository or download the `.ipynb` file.
2. Open the notebook in Jupyter, VSCode, or Google Colab.
3. Run each cell sequentially to reproduce the analysis.

---

