# FIFA21 Data Cleaning Pipeline

**Work In Progress** -Currently setting up project structure. Cleaning logic coming soon

ETL pipeline to clean FIFA21 player data.

## The Problem

Raw Kaggle FIFA21 dataset has inconsistent formats:
- Heights/weights as strings (**"5'11","165lbs"**)
- Currency values with abbreviations (**"$200k,","$15m"**)
- Newline characters in text fields
- Mixed string/numeric types in  **'Hits'** column.

## What This Does

1. Standardize physical measurements to numeric values.
2. Converts currency strings (K/M notation) to actual numbers.
3. Clean text formatting issues.
4. Output analysis-ready CSV.

- **Input:** 'data/raw/fifa21 raw data v2.csv'
- **Output:** 'data/processed/fifa21_clean_data.csv'

## Quick Start
### Requirements

- Docker & Docker Compose(for containerization execution)
- OR Python 3.8+ & pip (for local execution)

```bash
# Option 1: Using Docker
docker-compose up

# Option 2: Local Python
pip install -r requirements.txt
python main.py
```

## Tech Stack

- **Python/Pandas**: Data transformation
- **Docker**: Containerized environment for consistent execution**

