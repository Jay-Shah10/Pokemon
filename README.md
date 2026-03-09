# Pokemon Data Analytics

Exploratory data analysis of Pokemon stats for Generation 1 & 2 using Python and Jupyter.

## Dataset

[Pokemon Stats and Types — Generation 1 & 2 (Kaggle)](https://www.kaggle.com/datasets/nudratabbas/pokmon-stats-and-types-generation-1-2-index)

The dataset (`pokemon_stats_2025.csv`) contains 250 Pokemon with the following columns:

| Column | Description |
|---|---|
| `pokedex_id` | National Pokedex number |
| `name` | Pokemon name |
| `height` | Height (decimetres) |
| `weight` | Weight (hectograms) |
| `base_experience` | Base XP gained when defeated |
| `type_1` | Primary type |
| `type_2` | Secondary type (nullable) |
| `hp` | Hit points |
| `attack` | Physical attack |
| `defense` | Physical defense |
| `special_attack` | Special attack |
| `special_defense` | Special defense |
| `speed` | Speed |

## Analysis

The main notebook (`main.ipynb`) covers:

- Data exploration: shape, dtypes, null counts, descriptive stats
- Top 10 Pokemon by total stats
- Stat leaders per category (HP, Attack, Defense, etc.)
- Average stats grouped by primary type
- Single-type vs dual-type Pokemon comparison

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook main.ipynb
```

## Requirements

- Python 3.x
- pandas
- polars
- jupyter
