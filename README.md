# Premier League Prediction Model 2023

Predicted match outcomes for Premier league matches in the 2023-2024 season utilizing data scraped from the website: [https://fbref.com/en/comps/9/Premier-League-Stats](https://fbref.com/en/comps/9/Premier-League-Stats). Data scraping and prediction modelling done in Jupyter Notebook.

## Data Collection Through Web Scraping
Match data was scraped in `scrapingfbref.ipynb` using the main Python libraries: requests, BeautifulSoup and Pandas. Each Premier League team's data was stored in a DataFrame and merged. Scraped data was concised to include essential information and converted to a CSV file `matchstats.csv` in preparation for predictive modelling.

## Prediction Model
Machine learning library scikit-learn was used in `predictionmodel.ipynb` for data analysis of `matchstats.csv`. Random Forest algorithm was applied to assess training data, providing an accuracy outcome of 55.4% based on the 317 matches played up to date. Rolling average statistical method was also used to compare accuracy, resulting in a 50% outcome.  



