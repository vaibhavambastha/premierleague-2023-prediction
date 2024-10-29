# Premier League Prediction Model

As of January, 2024 half of the 2023/2024 season has been played. Utilizing match statistics of all matches played so far in the season, I constructed a prediction model for the remaining matches in the season. Match outcomes were predicted utilizing match statistics scraped from the open-source website: [https://fbref.com/en/comps/9/Premier-League-Stats](https://fbref.com/en/comps/9/Premier-League-Stats).

## Data Collection
- **Web Scraping**: Executed in `scrapingfbref.ipynb` using `requests`, `BeautifulSoup`, and `Pandas`.
- **Data Storage**: Each team’s data was organized in Pandas DataFrames and merged into a single dataset.
- **Data Preparation**: Essential match information was extracted, refined, and saved to `matchstats.csv` for model training.

## Prediction Model
- **Modeling Library**: Utilized `scikit-learn` in `predictionmodel.ipynb` for data analysis and prediction.
- **Features Considered**: Goals for/against, shooting stats, freekick/penalty rates, home/away outcomes, and expected goals.
- **Algorithm**: Applied the Random Forest algorithm for training, achieving a 55.4% accuracy based on 317 matches.
- **Rolling Average Method**: Integrated for further accuracy validation, with plans to update results as more data becomes available throughout the season.

## Files
- **`scrapingfbref.ipynb`**: Notebook for web scraping match statistics.
- **`matchstats.csv`**: Consolidated match data for model training.
- **`predictionmodel.ipynb`**: Notebook for prediction model development and testing.



