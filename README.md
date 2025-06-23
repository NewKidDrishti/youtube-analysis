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
* **Interactive Visualizations:** Many plots are generated using Plotly Express, offering interactive features for deeper exploration.

## Dataset

The analysis uses daily trending YouTube video data from the **United States**, sourced from Kaggle.

**Included Files (if downloaded locally):**
* `Youtube_Analysis_drishti.ipynb`: The main Jupyter Notebook with all code and analysis.
* `USvideos.csv`: The primary dataset of trending videos.
* `US_category_id.json`: Maps YouTube category IDs to names.

## Tools & Technologies

This project uses Python and the following libraries:

* **pandas:** For data manipulation and analysis.
* **numpy:** For numerical operations.
* **matplotlib:** For static visualizations.
* **seaborn:** For enhanced statistical data visualizations.
* **plotly:** For interactive visualizations.
* **wordcloud:** For generating word clouds.
* **scikit-learn:** For machine learning tasks (preprocessing, model training, evaluation).
* **kagglehub:** For downloading datasets directly from Kaggle.
* **collections** (built-in Python module)
* **re** (built-in Python module for regular expressions)
* **Jupyter Notebook:** The environment where the analysis and code are presented.

## How to Run the Analysis

1.  **Clone the Repository:**
    ```bash
    git clone [Your_GitHub_Repo_URL]
    cd [Your_GitHub_Repo_Name]
    ```
2.  **Install Libraries:**
    It's recommended to create a virtual environment first:
    ```bash
    # Optional: Create a virtual environment
    # conda create -n youtube_env python=3.9
    # conda activate youtube_env
    # Or: python -m venv youtube_env
    #     source youtube_env/bin/activate # macOS/Linux
    #     youtube_env\Scripts\activate # Windows
    ```
    Then, install the necessary packages:
    ```bash
    pip install pandas numpy matplotlib seaborn plotly wordcloud scikit-learn kagglehub
    ```
3.  **Acquire Data:**
    If you don't have the `USvideos.csv` and `US_category_id.json` files locally, you can download them using `kagglehub`. **Note:** You will need to have your Kaggle API credentials set up for this to work (usually `kaggle.json` in `~/.kaggle/`).
    ```python
    import kagglehub

    # Download latest version of the 'youtube-new' dataset
    # This will download the files to a local directory (e.g., ~/.kaggle/datasets/datasnaek/youtube-new/...)
    path = kagglehub.dataset_download("datasnaek/youtube-new")

    print("Path to dataset files:", path)
    ```
    Alternatively, you can manually download `USvideos.csv` and `US_category_id.json` from the [Kaggle YouTube New Trending Videos dataset page](https://www.kaggle.com/datasets/datasnaek/youtube-new) and place them in your project folder.
4.  **Launch Jupyter Notebook:**
    Ensure `Youtube_Analysis_drishti.ipynb`, `USvideos.csv`, and `US_category_id.json` are in the same folder.
    ```bash
    jupyter notebook
    ```
5.  **Run the Notebook:** Open `Youtube_Analysis_drishti.ipynb` and execute all cells sequentially (`Cell > Run All`).

## Key Insights

* **Fast Trending is Key:** The vast majority of videos hit the trending list within 0-2 days of being published, highlighting the importance of immediate virality.
* **Content Categories Matter:** Entertainment, Music, and News & Politics frequently dominate the trending charts, indicating high audience interest in these areas.
* **Views Drive Engagement, But Ratios Tell More:** While high views correlate with more likes and comments, the "likes per view" and "comments per view" ratios can highlight highly engaging or polarizing content, even with lower view counts.
* **Strategic Publishing Times:** There are specific hours and days of the week when videos are more likely to trend, suggesting optimal publishing windows.

---
