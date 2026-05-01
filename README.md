# Handmade Products Recommendation Project

This repository contains data preprocessing, sparsity simulation, and recommendation model experiments using MovieLens and handmade product ratings.

## Repository structure

- `data/raw/` — raw dataset files
- `notebooks/` — Jupyter notebooks for preprocessing and modeling
- `plots/` — generated figures
- `results/` — evaluation CSV outputs
- `saved/` — serialized cleaned datasets used across notebooks
- `requirements.txt` — Python dependencies
- `.gitignore` — files and folders excluded from version control

## Recommended setup

1. Open this folder in VS Code.
2. Select the Python interpreter for the workspace virtual environment:
   - `./.venv/bin/python`
   - Use `Python: Select Interpreter` from the command palette if needed.
3. Install dependencies if not already installed:
   ```bash
   ./.venv/bin/python -m pip install -r requirements.txt
   ```
4. Open `notebooks/01_data_preprocessing.ipynb` and run it first.
5. Then open `notebooks/02_modeling.ipynb` and run it next.

## Running the notebooks

- `notebooks/01_data_preprocessing.ipynb` loads raw data from `data/raw/`, cleans it, generates EDA plots, and saves the cleaned datasets to `saved/`.
- `notebooks/02_modeling.ipynb` loads the cleaned datasets from `saved/` if available, or rebuilds them from `data/raw/` as a fallback.

## Docs

- See `docs/overview.md` for a short project summary and recommended workflow.

## Troubleshooting

- Verify the notebook kernel is using the workspace `.venv`.
- If imports fail, run:
  ```bash
  ./.venv/bin/python -m pip install -r requirements.txt
  ```
- If the data files are missing, make sure `data/raw/` contains:
  - `Handmade_Products.jsonl`
  - `ratings.dat`
  - `movies.dat`
  - `users.dat`

## Notes

- The `plots/`, `results/`, and `saved/` folders are generated output and are excluded from git.
- The raw datasets are stored in `data/raw/` to keep the repository organized.
