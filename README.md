Movie Dataset Exploratory Data Analysis
# Overview

This project examines a movie dataset through univariate and bivariate analysis. It explores patterns in ratings, budgets, revenues, scores, and director activity to understand the factors driving box-office performance.

# Objectives

Analyze movie trends across ratings, genres, budgets, and earnings

Study relationships between budget, gross revenue, score, and votes

Identify top directors and dominant categories

Detect missing or inconsistent data

Summarize insights that influence movie success

# Key Analyses

Rating distribution

Genre and director frequency

Budget, gross, score, and vote distributions

Budget vs Gross

Score vs Votes

Yearly revenue trends

Correlation heatmap

# Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

# Movies Directed by S. S. Rajamouli (Telugu Cinema Highlights)

This filter shows the two landmark Telugu films directed by S. S. Rajamouli in the dataset:
Baahubali: The Beginning (2015) and Baahubali 2: The Conclusion (2017).
Both films represent some of the biggest productions in Indian cinema, with massive budgets and exceptional box-office performance. Starring Prabhas and written by Vijayendra Prasad, these films set new benchmarks for storytelling, scale, and visual effects in Telugu industry. Their high scores and strong audience engagement reflect the impact these movies created across India and worldwide.

# 📊 Detailed Chart Explanations
1. Heatmap – Budget, Gross, Votes, Score Correlations

This heatmap shows how the key numerical variables relate to each other.
The strongest relationship is between budget and gross revenue, confirming that higher investment usually leads to higher box-office returns. Votes also correlate well with gross, indicating that popular movies with large audiences tend to earn more. Scores show moderate alignment with votes but weak connection with earnings. Year and runtime add minimal explanatory value.
This chart helps identify which features matter most for predicting movie success.

2. Rating Distribution – Bar Chart

This chart visualizes how movies are spread across rating categories.
R-rated films have the highest frequency, reflecting adult-oriented content dominance. PG-13 and PG movies also appear in large numbers, representing family and teen-friendly productions. Very few titles fall under G, TV ratings, or NC-17. The presence of “Not Rated” entries reveals inconsistency in rating data, which may require cleaning before modeling.
This distribution provides a clear understanding of content classification trends.

3. Top 10 Directors – Bar Chart

This chart ranks directors by the number of movies they contributed.
Woody Allen appears most frequently, followed by Clint Eastwood and Steven Spielberg. These directors show consistent output across decades. However, mislabeled entries such as “Directors” point to inaccuracies in the dataset. The distribution also highlights how only a handful of directors produce a significant number of films, while most contribute very few.
This gives insight into creative influence and dataset reliability.

4. Gross Revenue by Year – Line Chart

This line chart highlights long-term changes in movie earnings.
Gross revenue steadily rises from the early 1980s to around 2018, with a sharp upward trend during the mid-2000s as overall production and budgets increased. A sudden decline in 2020 aligns with industry disruptions like reduced theatrical releases.
This visualization demonstrates how external factors and industry growth impact financial performance over time.

5. Score vs Votes – Scatter Plot

This scatter plot shows how user scores relate to the number of votes.
Movies with more votes tend to have higher and more stable scores, showing that audience engagement strengthens rating reliability. Low-vote films display wide variation, indicating inconsistent or biased scoring. A few outliers received many votes despite average scores.
This chart explains how audience size affects rating accuracy.

6. Budget vs Gross Earnings – Scatter Plot

This plot examines how financial investment impacts box-office results.
There is a clear positive relationship: movies with larger budgets typically earn more. Low-budget films show unpredictable outcomes—some perform poorly while others exceed expectations. High-budget films cluster near high-gross values, making them more dependable performers.
A few high-budget outliers fail to generate returns, revealing financial risk.
This visualization is critical for understanding economic drivers of movie success.

# How to Use

Clone the repository

Install the required libraries

Open the notebook and run the cells in order

# Conclusion

The analysis reveals clear trends in how movies perform. Higher budgets often result in higher gross earnings, audience engagement aligns with stronger scores, and yearly revenue trends show long-term growth with occasional dips. A few genres and directors dominate the dataset, while data-quality issues highlight the need for careful cleaning
