# 🎬 Movie Dataset — Exploratory Data Analysis (EDA)

A data analysis project that explores patterns in a large movie dataset, uncovering the key factors that drive box-office success — from budgets and genres to directors and audience ratings.

---

## 📌 Problem Statement

The dataset contains information about movies across different years, genres, budgets, revenues, ratings, and creators. The goal is to understand patterns that influence a movie's performance and identify the key factors that drive box-office success.

---

## 🎯 Objectives

- Analyze the distribution of movie ratings, genres, budgets, and earnings
- Identify trends in gross revenue over the years
- Measure the relationship between budget, gross earnings, votes, and scores
- Highlight top-performing directors and countries with the most movie output
- Detect data quality issues such as missing or inconsistent entries

---

## 📂 Project Structure

```
├── project_EDA.ipynb             # Main Jupyter Notebook with full analysis
├── project_ppt.pptx              # Presentation summarizing key findings
├── movies.csv                    # Dataset (not included — see below)
├── images/
│   ├── correlation_heatmap.png   # Correlation matrix heatmap
│   └── rating_distribution.png  # Movie rating bar chart
└── README.md
```

---

## 📊 Dataset

The dataset (`movies.csv`) contains the following key features:

| Column | Description |
|--------|-------------|
| `name` | Movie title |
| `rating` | MPAA rating (G, PG, PG-13, R, etc.) |
| `genre` | Primary genre |
| `year` | Release year |
| `released` | Full release date |
| `score` | IMDb score |
| `votes` | Number of audience votes |
| `director` | Director name |
| `writer` | Writer name |
| `budget` | Production budget (USD) |
| `gross` | Gross box-office earnings (USD) |
| `country` | Country of production |
| `company` | Production company |
| `runtime` | Movie duration (minutes) |

> ⚠️ The dataset is not included in this repository. You can download a similar dataset from [Kaggle — Movies Dataset](https://www.kaggle.com/).

---

## 🛠️ Technologies Used

- **Python 3**
- **Pandas** — data loading, cleaning, and manipulation
- **NumPy** — numerical operations
- **Matplotlib** — base visualizations
- **Seaborn** — statistical plots and heatmaps

---

## 🔍 Analysis Performed

### 1. Data Cleaning
- Converted `budget` and `gross` to numeric types
- Filled missing budget and gross values with the column median
- Filled missing ratings with `'unknown'`
- Filled missing runtime with the column median
- Stripped whitespace from categorical columns

### 2. Visualizations & Key Insights

#### 📈 Budget vs. Gross Earnings (Scatter Plot + Regression)
- Higher budgets generally lead to higher gross earnings — a clear positive relationship
- Low-budget films show high variance; some small productions outperform expectations
- A few high-budget outliers failed to convert investment into strong earnings

#### 🌡️ Correlation Heatmap (Numeric Features)

![Correlation Matrix Heatmap](images/correlation_heatmap.png)

- **Budget ↔ Gross: 0.75** — strong positive correlation
- **Votes ↔ Gross: 0.63** — audience engagement significantly impacts earnings
- Score shows moderate correlation with votes but weak correlation with gross
- Year and runtime have minimal influence on box-office performance

#### ⭐ Score vs. Votes (Scatter Plot)
- Movies with higher vote counts tend to have higher scores
- Low-vote movies show wide score variation — ratings are less reliable
- A few outliers received many votes despite only average scores

#### 📅 Gross Revenue by Year (Line Chart)
- Steady revenue growth from the early 1980s through ~2018
- Sharp acceleration after the mid-2000s
- Notable revenue drop in 2020 due to industry disruption

#### 🎭 Movie Rating Distribution (Bar Chart)

![Movie Rating Distribution](images/rating_distribution.png)

- **R-rated movies dominate** the dataset
- PG-13 and PG follow with strong representation
- Very few G, NC-17, or TV-rated films
- A notable number of entries are missing or labeled "Not Rated"

#### 🎬 Top 10 Directors by Movie Count
- **Woody Allen** leads with the highest movie count
- Clint Eastwood and Steven Spielberg follow closely
- Reveals that prolific output is concentrated among a small group of directors

#### 🌍 Country-Wise Movie Count
- A small number of countries — led by the USA — dominate movie production output

---

## ✅ Conclusions

- Higher budgets reliably lead to higher box-office earnings
- Audience engagement (votes) aligns closely with both higher scores and greater revenue
- Revenue has grown steadily over the decades, with notable disruption in 2020
- Rating and genre distributions show that a few categories dominate production
- Only a small group of directors appear consistently across the dataset
- Data quality gaps (missing ratings, inconsistent labels) need cleaning before deeper modeling

---

##  Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Run the Notebook

```bash
git clone https://github.com/your-username/movie-eda.git
cd movie-eda
jupyter notebook project_EDA.ipynb
```

>  `movies.csv` file in the root directory 
> "C:\Users\SINDHU\Downloads\project_EDA.ipynb"

---

##  Contact

Made with ❤️ for data exploration.  
Feel free to open an issue or submit a pull request!


