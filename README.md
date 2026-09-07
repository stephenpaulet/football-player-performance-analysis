# Football Player Performance Analysis

Exploratory data analysis of 2025-2026 top-5 European league player stats (FBref), covering goal output, per-90 efficiency, age trends, and positional comparisons using Python, Pandas, and Seaborn.

## What this is

A short, honest exploratory analysis of real player-level football data from the Premier League, La Liga, Bundesliga, Serie A, and Ligue 1. Built as a personal project to practice the full analysis workflow: loading, cleaning, feature engineering, visualization, and drawing plain-language conclusions from the results.

## Dataset

[Football Players Stats (2025-2026)](https://www.kaggle.com/datasets/hubertsidorowicz/football-players-stats-2025-2026) by Hubert Sidorowicz, sourced from [FBref](https://fbref.com).

The dataset uses standard FBref abbreviations:
- `Gls` = Goals
- `Ast` = Assists
- `Min` = Minutes played
- `90s` = Minutes / 90 (already pre-calculated)
- `Pos` = Position
- `Squad` = Club
- `Comp` = League / Competition

## What's in this repo

- the full notebook: data loading, cleaning, feature engineering, charts, and findings `football_analysis.ipynb`.
- A static, no-setup export of the notebook and its output `football_analysis.pdf`

The raw dataset CSV is **not included** in this repo (see below).

## How to run it

1. Download `players_data-2025_2026.csv` from the [Kaggle dataset page](https://www.kaggle.com/datasets/hubertsidorowicz/football-players-stats-2025-2026).
2. Place it in the same folder as `football_analysis.ipynb`.
3. Run all cells. The notebook expects the real CSV to be present. If it's missing, it raises a clear error telling you where to get it, rather than instantly failing.

## What the analysis covers

1. First look at the data (shape, types, missing values...)
2. Cleaning (dropping zero-minute rows, trimming to the relevant columns)
3. Feature engineering (goals and assists per 90 minutes)
4. Top goal scorers
5. Goal contributions by position
6. Age vs. per-90 output
7. Plain-language findings

## Why the dataset isn't in this repo

FBref's underlying data is scraped from a third-party source, and the Kaggle dataset's exact redistribution terms are not clearly documented.

## Tools used

Python, Pandas, Matplotlib, Seaborn.
