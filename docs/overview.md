# Handmade Products Recommendation Project

This repository contains a small recommender system case study using MovieLens data and a handmade products dataset.

## Structure

- `data/raw/` — raw input files used for preprocessing and experiments.
- `notebooks/01_data_preprocessing.ipynb` — cleans the datasets, runs exploratory data analysis, and saves cleaned outputs.
- `notebooks/02_modeling.ipynb` — loads the cleaned datasets, runs sparsity and evaluation experiments, trains models, and saves results.
- `plots/` — generated chart images.
- `results/` — exported CSV summaries of model performance.
- `saved/` — serialized cleaned datasets for reuse across notebooks.

## How to use

1. Open `notebooks/01_data_preprocessing.ipynb` and run it first.
2. After it finishes, open `notebooks/02_modeling.ipynb` and run it.

This keeps the workflow clear: first preprocess and save, then build and evaluate models.
