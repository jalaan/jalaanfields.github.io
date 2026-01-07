# jalaanfields.github.io
Data Science Projects 
# Netflix-Style Analytics Platform (End-to-End Data Project)

## Overview
This project simulates a real-world streaming analytics platform similar to Netflix.
It demonstrates data engineering, analytics engineering, and visualization using
modern tools and best practices.

## Architecture
Ingestion (Python) → Data Lake (Parquet) → Warehouse (DuckDB) → dbt Models → Dashboard (Streamlit)

## Tech Stack
- Python (Pandas, Faker)
- SQL
- DuckDB
- dbt (analytics engineering)
- Parquet
- Streamlit

## Key Features
- 200K+ simulated streaming events
- Partitioned data lake
- Star-schema analytics models
- dbt tests for data quality
- Interactive KPI dashboard

## Business Questions Answered
- Daily active users
- Content engagement trends
- Top-performing titles
- Buffering and watch-time analysis

## How to Run
```bash
python src/generate_events.py
python src/ingest_to_lake.py
python src/load_to_duckdb.py
dbt build
streamlit run dashboard/app.py
