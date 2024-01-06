# AFCON 2023 Data Analysis and Prediction

This project scrapes data for the Africa Cup of Nations (AFCON) 2023, a biennial African association football tournament organised by Confederation of African Football (CAF). It then cleans up the data and performs some exploratory data analysis and prediction using Python and Jupyter Notebook.

## Overview

The AFCON 2023 is scheduled to take place from 13 January to 11 February 2024 in Ivory Coast. It will be the 34th edition of the tournament and the second time that Ivory Coast hosts the finals. The tournament will feature 24 teams that qualified from the preliminary rounds.

The aim of this project is to collect and analyze data related to the AFCON 2023, such as the teams, fixtures, results, and statistics. The project also attempts to predict the outcome of the matches and each round of the tournament using historical data and the Poisson distribution.

## Features

- Data scraping: The project uses the requests and BeautifulSoup libraries to scrape historical, fixture, and groups data from Wikipedia. The data is then stored in CSV files for further processing, while the groups are dumped as binary (with pickle).
- Data cleaning: The project uses the pandas library to clean and manipulate the data, such as removing duplicates, handling missing values, and merging data frames.
- Data prediction: The project uses the Poisson distribution to model the number of goals scored by each team in a match, and then calculates the probabilities of different outcomes, such as win, draw, or loss. The project also uses the points system to rank the teams and predict the winner of the tournament.

## Installation

The following packages are required to run the code in this repository:

- pandas, beautifulsoup4, requests, time, pickle, scipy, numpy

1. Clone this repository to your local machine.
2. Install the required dependencies using the following command:

```bash
pip install -r requirements.txt
```

## Dataset

The dataset for this project can be found in the `/data` folder, and consists of several CSV files that contain data scraped from Wikipedia related to the AFCON 2023, such as:

- afcon_historical_data_clean.csv: This file contains historical data of all the AFCON tournaments from 1957 to 2021, such as the year, host, winner, runner-up, third place, fourth place, number of teams, number of matches, number of goals, etc.
- afcon_fixture_data_clean.csv: This file contains fixture data of the AFCON 2023, such as the date, time, group, team 1, team 2, and venue of each match.
- afcon_groups_data.csv: This file contains group data of the AFCON 2023, such as the group, team, rank, points, played, won, drawn, lost, goals for, goals against, and goal difference of each team in each group.
- afcon_groups_dump.csv: This file contains a dump of the table of the AFCON 2023 groups from Wikipedia as a dictionary, which was used to make analysis easier to parse.

## Notebooks

This repository contains two Jupyter Notebook files that shows the steps and codes for data scraping, cleaning, analysis, visualization, and prediction. The notebook also contains comments and explanations for each step and code. The notebook can be viewed online using GitHub or nbviewer, or downloaded and run locally using Jupyter Notebook.

## Conclusion

This project demonstrates how to use Python and Jupyter Notebook to scrape, clean, analyze, visualize, and predict data for the AFCON 2023. The project also provides some insights and findings about the tournament, such as:

- The most successful team in AFCON history is Egypt, with seven titles, followed by Cameroon, with five titles, and Ghana, with four titles1
- The highest-ranked team in the tournament is Senegal, ranked 20th in the world, followed by Tunisia, ranked 25th, and Algeria, ranked 30th2
- The most likely outcome of the group stage is that Senegal, Tunisia, Algeria, and Cameroon will top their respective groups, while Ivory Coast, Morocco, Nigeria, and Ghana will finish second
- The most likely winner of the tournament is Egypt based on historical performance and average points in previous fixtures.

The project also has some limitations and challenges, such as:

- The data scraping process depends on the structure and availability of the websites, which may change over time and affect the quality and quantity of the data.
- The data cleaning and manipulation process involves some assumptions and decisions, which may introduce some errors and biases in the data.
- The data analysis and visualization process involves some choices and parameters, which may affect the interpretation and presentation of the data.
- The data prediction process involves some models and methods, which may have some limitations and assumptions, and may not generalize well to new data.

The project can be improved and extended in several ways, such as:

- Scraping more data from other sources, such as social media, news articles, and betting odds, to enrich the dataset and provide more features and perspectives.
- Analyzing and visualizing the data more deeply and creatively, to explore more patterns and relationships in the data and generate more insights and findings.
- Predicting the data more accurately and robustly, to use more advanced and sophisticated models and methods, and to evaluate and compare their performance and results.
- Using artificial intelligence, or machine learning models to predict the outcomes based on several parameters, not only the historical goals and points.
