# Pokemon Data Analytics Project

## Project Overview
Exploratory data analysis of Pokemon stats using a Jupyter notebook (`main.ipynb`) and a CSV dataset (`pokemon_stats_2025.csv`).

## Environment Setup

### Python Virtual Environment
A `.venv` directory is present at the project root. Activate it before running anything:

```bash
source .venv/bin/activate
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

### Run the Notebook
```bash
jupyter notebook main.ipynb
```

## Project Structure
```
Pokemon/
├── .venv/                   # Python virtual environment (do not commit)
├── main.ipynb               # Primary Jupyter notebook
├── pokemon_stats_2025.csv   # Dataset
├── requirements.txt         # Python dependencies
└── CLAUDE.md                # This file
```

## Key Libraries
- **pandas** — primary DataFrame library for data loading and exploration
- **polars** — high-performance DataFrame library (imported, available for use)

## Dataset
`pokemon_stats_2025.csv` — contains Pokemon stats with columns including type info. Notable: `type_2` has expected null values since not all Pokemon have a second type.

## Current Work
- Data exploration: shape, dtypes, null counts, descriptive stats, unique value counts
- Planned next steps (from notebook comments):
  - Create a new DataFrame with a `total_stats` column
  - Separate DataFrames for single-type and dual-type Pokemon

## Notes
- `os`, `sys`, and `datetime` are stdlib imports — no installation needed
- Do not commit `.venv/` to version control; add it to `.gitignore`
