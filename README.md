# 📊 Streaming Wars: Visualizing Competitive Trends in the OTT Industry

This project explores the evolving landscape of major streaming platforms — **Netflix**, **Prime Video**, **Hulu**, and **Disney+** — by analyzing trends in content volume, genre specialization, and critical reception from **2000 to 2021**. Through a set of interactive visualizations, we uncover how each platform competes in terms of quantity, quality, and strategic content curation.

---

## 📌 Objectives

- Analyze how the content volume has changed over time across platforms.
- Identify platform-specific genre strengths using Rotten Tomatoes ratings.
- Compare quantity vs. quality trade-offs through bubble plots.
- Explore internal genre distribution per platform.
- Deliver interactive, filterable visualizations for deeper insights.



## Dataset

- **Source**: [Kaggle Dataset - Movies on Netflix, Prime Video, Hulu, and Disney+](https://www.kaggle.com/datasets/ruchi798/movies-on-netflix-prime-video-hulu-and-disney)
- **Metadata Enrichment**: Genres and other missing fields were filled using the [TMDb API](https://developer.themoviedb.org/docs).
- **Updated dataset avaiable with the file name Movies_Full_With_Genres**
- **Coverage**: Titles released between **2000–2021**



## Tools and Technologies

| Tool         | Purpose                            |
|--------------|-------------------------------------|
| `Python`     | Core scripting and data analysis    |
| `Pandas`     | Data wrangling, merging, enrichment |
| `Altair`     | Interactive visualizations          |
| `Seaborn` & `Matplotlib` | Static visualizations       |
| `Jupyter Notebook` | Development and visualization environment |


## Visualizations

- **Stacked Area Chart**: Content volume growth by year and platform.
- **Heatmap**: Average Rotten Tomatoes ratings per genre by platform.
- **Interactive Bubble Plot**: Quantity vs. quality by genre across platforms.
- **Interactive Pie Chart**: Genre distribution per platform (filterable).
- **Bar Charts & Box Plots**: Additional breakdowns of genre and ratings.


## Key Insights

- Netflix leads in **content volume**, but **moderate ratings**.
- Disney+ focuses on **high-quality genres** like *Fantasy* and *Action*.
- Hulu excels in **niche genres** like *War*, *History*, and *Western*.
- Prime Video has a **balanced genre mix**, with *History* performing well.


## Limitations

- Dataset ends in **2021** — recent content and trends are not captured.
- Original content was inferred based on platform exclusivity.
- Some genre labels are broad and lack sub-genre granularity.
- Audience sentiment from IMDb/RT users not included (planned).


## Future Work

- Add sub-genre classification (e.g., Action-Comedy vs Psychological Thriller)
- Integrate audience ratings alongside critic scores.
- Expand dataset to include 2022–2024 and new entrants.
- Build a web-based dashboard for broader accessibility.


## File Structure

StreamingWars/
├── ML_classifications.ipynb        # Jupyter notebook with analysis, visualizations, and insights
├── README.md                       # Project overview and documentation
├── requirements.txt                # List of required Python packages
├── data/
│   ├── raw/                        # Original Kaggle dataset (CSV)
│   └── processed/                  # Cleaned and enriched dataset with TMDb metadata
├── assets/
│   ├── Heatmap.png                 # Exported heatmap of genre ratings
│   ├── BubbleChart.png            # Exported bubble plot
│   ├── PieChart.png               # Genre distribution donut chart
│   └── StackedAreaChart.png       # Platform content volume over time
├── utils/
│   └── api_tmdb_fetcher.py        # Script for fetching metadata using TMDb API
└── LICENSE                         # Project license (e.g., MIT)


## How to Run

 Clone the repository:
   ```bash
   git clone https://github.com/yourusername/StreamingWars.git
   cd StreamingWars
