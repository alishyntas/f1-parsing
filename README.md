# f1-parsing
Python script for scraping Formula 1 race data from formula1.com (race, practices, qualifying, race grid, pit stops, fastest laps, sprint, sprint grid).

------------------------------------------------------------------------------------------------------------------------------------------

# Formula 1 Data Scraper & Cleaning

Scraping full Formula 1 race weekend data: Race, Practice, Qualifying, Grid, Pit Stops, Fastest Laps, Sprint, Sprint Grid, Driver Standings, Team Standings.
This project automatically collects Formula 1 season data from the official formula1.com website, converts it into structured pandas DataFrames, and prepares it for the next step - data cleaning.
The script extracts results from all major race-weekend sessions and aggregates them into unified datasets.


------------------------------------------------------------------------------------------------------------------------------------------


# Features

✔️ Scrapes all races for a selected season

✔️ Practice sessions (P1, P2, P3)

✔️ Qualifying results

✔️ Starting grid positions

✔️ Sprint grid (for seasons with sprint races)

✔️ Pit stop summary

✔️ Fastest laps

✔️ Sprint

✔️ Sprint Grid

✔️ Driver Standings

✔️ Team Standings



------------------------------------------------------------------------------------------------------------------------------------------

# Libraries

BeautifulSoup4 — HTML parsing

requests — HTTP requests

pandas — data manipulation

numpy — helper tools


------------------------------------------------------------------------------------------------------------------------------------------

# Changing Year 

You can change the year variable to any other dates, and it will parse the data for the specified year.

year = 2021

url = f"https://www.formula1.com/en/results/{year}/races"

resp = requests.get(url)

soup = BeautifulSoup(resp.text, "html.parser")



