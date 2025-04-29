# IMDB Movies SQL Analysis

This project explores a dataset of 250 top-rated IMDB movies using SQL queries via DuckDB and Python, with results displayed as interactive tables using [itables](https://mwouts.github.io/itables/). The report is written in a [Quarto](https://quarto.org/) `.qmd` notebook.

## Features

- Query and analyze movie data using SQL
- Display results as interactive HTML tables
- Powered by DuckDB, itables, and Quarto

## Installation

1. Clone the repository:

```bash
git clone https://github.com/gpenessot/imdb-sql-analysis.git
cd imdb-sql-analysis
```

2. Create a virtual environment and install dependencies using [`uv`](https://github.com/astral-sh/uv):

```bash
uv venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows
uv pip install -r pyproject.toml
```

## Usage

To render the Quarto notebook as HTML:

```bash
quarto render notebook.qmd
```

Or open it interactively in Jupyter:

```bash
quarto preview notebook.qmd
```

## Dataset

The SQLite database `movies.db` should be placed inside the `data/` folder. It must contain a `movies` table with the following columns:

- `title`, `director`, `year`, `rating`, `genres`, `runtime`, `country`, `language`, `imdb_score`, `imdb_votes`, `metacritic_score`

## License

MIT License
