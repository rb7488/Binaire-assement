# PICO-8 Game Dataset Scraper

## Overview

This project is part of the Machine Learning Assessment for **Binaire Private Limited**.

The objective of Task 2 is to scrape the first 100 PICO-8 games/cartridges from the Lexaloffle BBS and create a structured CSV dataset containing information about each game.

The scraper is implemented in Python using `requests`, `BeautifulSoup`, and `pandas`.

## Source

The data is collected from the PICO-8 Cartridges section of the Lexaloffle BBS:

https://www.lexaloffle.com/bbs/?cat=7&carts_tab=1&sub=2&mode=carts

## Features Collected

For each game, the scraper attempts to collect:

- **Game Name** – Name/title of the PICO-8 game
- **Author** – Creator of the game
- **Game Artwork** – URL of the game's artwork/thumbnail
- **Game Code** – PICO-8 source code retrieved from the cartridge snippet endpoint
- **License** – License specified by the game author
- **Like Count** – Number of likes
- **Game Description** – Description/content associated with the game
- **Top 5 Comments** – Up to five comments from the game discussion
- **Game URL** – Original Lexaloffle BBS page
- **Cart ID** – PICO-8 cartridge identifier

## Technologies Used

- Python 3
- Requests
- BeautifulSoup4
- Pandas
- lxml
- Regular Expressions

## Project Structure

```text
task-2-pico8-scraper/
│
├── scraper.py
├── pico8_first_100_games.csv
├── README.md
└── requirements.txt
