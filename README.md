# Hit Formula: Audio Characteristics That Shaped 1990s Classic Songs

**End-to-end data analysis** exploring audio features that correlate with popularity in 1990s hit songs.
Built with **Python (Pandas)** for cleaning, **MySQL** for analysis, and **Tableau Public** for visualization.

---

## Project Summary
This project investigates what audio characteristics (tempo, energy, danceability, key, acousticness, etc.) were common among popular 1990s songs. It demonstrates a full analyst workflow: data cleaning, DB design & SQL analysis, and visual storytelling.

**Key questions:**
- Which audio features are most strongly associated with popularity?
- Are there tempo / energy “sweet spots” for hits?
- How did musical characteristics change across the decade?

---

## Repo structure
```
90s-Hits-Data-Analysis/
├── data/
│   ├── raw/1990sClassicHits.csv
│   └── cleaned/1990sClassicHits_clean.csv
├── notebooks/
│   └── data_cleaning.ipynb
│   └── exploratory_analysis.ipynb
├── scripts/
│   └── clean_data.py
├── sql/
│   ├── create_tables.sql
│   ├── load_data.sql
│   └── analysis_queries.sql
├── tableau/
│   └── dashboard_screenshots/
│   └── tableau_public_links.txt
├── images/
│   └── repo_banner.png
├── README.md
└── LICENSE
```

---

## How to run
1. Inspect raw data: `data/raw/1990sClassicHits.csv`  
2. Run the cleaning notebook: `notebooks/data_cleaning.ipynb` (or `python scripts/clean_data.py`)  
3. Load cleaned CSV into MySQL using `sql/load_data.sql` (adjust path)  
4. Run `sql/analysis_queries.sql` to generate aggregated tables and CSV outputs for Tableau  
5. Build dashboards in Tableau Public and publish

---

## Notable files
- `notebooks/data_cleaning.ipynb` — step-by-step cleaning & feature engineering  
- `sql/create_tables.sql` — MySQL schema  
- `sql/analysis_queries.sql` — all analysis queries (deciles, correlations, trends)  
- `tableau/` — packaged dashboard screenshots and links

---

## Key insights (examples - update after analysis)
- Popular songs tend to be between **120–135 BPM**.  
- High-energy tracks (energy > 0.65) are overrepresented among top popularity scores.  
- Songs in **major keys** (mode=1) have slightly higher average popularity.  
- Acoustic tracks tend to have lower popularity on average.

---

## Technologies
- Python (Pandas, NumPy, Matplotlib)  
- MySQL  
- Tableau Public  
- Jupyter Notebook

---

## Next steps & extensions
- Enrich with Spotify API metadata (genre, album)  
- Build a simple ML model to predict popularity deciles  
- Create a Streamlit app to interactively test “hit” profiles

---

## Author
Dann Jeffries
Your Name — Junior Data Analyst portfolio project  
Contact: youremail@example.com
