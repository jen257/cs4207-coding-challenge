# CS4207 Coding Challenge — Group 4

## Project Overview
- **Module:** CS4207 — Advanced Programming Concepts and Practices (2026/27 Sem 1)
- **Task:** Payment Method Classification (Credit Card vs. Cash)
- **Dataset:** 2026 NYC Yellow Taxi Trip Records (Parquet format, Jan–Apr 2026)
- **Team Members (Group 4):**
  - JiaLiang Lyu
  - HuiLin Chong
  - JiaDong Chen
  - Bei Yu
  - Cheng Yang

## Repository Structure
- `CS4207_Group4.ipynb` — Main solution notebook covering all 6 assessment criteria (data cleaning, data parallelism, task parallelism, benchmarking, non-determinism fixes, and reproducibility).
- `requirements.txt` — Python package dependencies.
- `.gitignore` — Excludes large `.parquet`/`.tar.gz` dataset files, local shards, and virtual environments.

## How to Run

### 1. On Google Colab (Development)
1. Upload `yellow_tripdata_2026-01.parquet` through `yellow_tripdata_2026-04.parquet` to Google Drive under `MyDrive/CS4207/`.
2. Open `CS4207_Group4.ipynb` in Google Colab and run all cells.

### 2. On CSIS Rockhill Server (Final Benchmarks — Mandatory)
The dataset is already available on Rockhill at `/home/cs4207/data/`.
```bash
# Activate virtual environment
source ~/envs/myenv/bin/activate

# Install dependencies if needed
pip install -r requirements.txt

# Execute notebook on Rockhill
jupyter nbconvert --to notebook --execute --inplace CS4207_Group4.ipynb
