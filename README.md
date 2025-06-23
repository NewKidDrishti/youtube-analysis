# YouTube Trending Video Analysis & Engagement Prediction

## Project Overview

This project analyzes daily trending YouTube video data from the US to uncover patterns, trends, and factors contributing to video popularity and engagement. It includes extensive data cleaning, exploratory data analysis, and a machine learning model to predict high engagement.

## Key Features

* **Data Cleaning & Feature Engineering:** Preprocessing raw data and creating new metrics (e.g., engagement ratios).
* **Exploratory Data Analysis (EDA):** Insights into video categories, views, likes, and comments distributions.
* **Trending Dynamics:** Analysis of how long videos trend and the time taken to hit trending.
* **Content Analysis:** Word clouds from video titles and tags.
* **Channel Performance:** Deep dive into top-performing channels.
* **Time Series Trends:** Daily and hourly patterns of trending videos.
* **Machine Learning:** A classifier to predict videos with high engagement based on features.

## Dataset

The analysis uses daily trending YouTube video data from the **United States**.

**Included Files:**
* `Youtube_Analysis_drishti.ipynb`: The main Jupyter Notebook with all code and analysis.
* `USvideos.csv`: The primary dataset of trending videos.
* `US_category_id.json`: Maps YouTube category IDs to names.

## Tools & Technologies

* Python
* Pandas (Data Manipulation)
* NumPy (Numerical Operations)
* Matplotlib, Seaborn, Plotly (Visualizations)
* WordCloud (Text Analysis)
* Scikit-learn (Machine Learning)
* Jupyter Notebook

## How to Run the Analysis

1.  **Clone the Repository:**
    ```bash
    git clone [Your_GitHub_Repo_URL]
    cd [Your_GitHub_Repo_Name]
    ```
2.  **Install Libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn plotly scikit-learn wordcloud jupyter
    ```
3.  **Launch Jupyter Notebook:**
    Ensure `Youtube_Analysis_Drishti.ipynb`, `USvideos.csv`, and `US_category_id.json` are in the same folder.
    ```bash
    jupyter notebook
    ```
4.  **Run the Notebook:** Open `Youtube_Analysis_drishti.ipynb` and execute all cells sequentially (`Cell > Run All`).

## Key Insights

* **Fast Trending is Key:** The vast majority of videos hit the trending list within 0-2 days of being published, highlighting the importance of immediate virality.
* **Content Categories Matter:** Entertainment, Music, and News & Politics frequently dominate the trending charts, indicating high audience interest in these areas.
* **Views Drive Engagement, But Ratios Tell More:** While high views correlate with more likes and comments, the "likes per view" and "comments per view" ratios can highlight highly engaging or polarizing content, even with lower view counts.
* **Strategic Publishing Times:** There are specific hours and days of the week when videos are more likely to trend, suggesting optimal publishing windows.

---
