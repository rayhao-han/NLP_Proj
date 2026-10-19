# CITS4012 Group 56: MultiRC

Everything is in `CITS4012_Group56.ipynb`. Its Readme cell describes dependencies, settings and run time.

**Google Colab:** open the notebook, choose a GPU runtime (T4) and use *Runtime → Run all*. The first code cell
clones this repository into `/content/NLP_Proj` and works from there, so the data, checkpoints and saved
results are found automatically and nothing is retrained.

**Locally:** `python -m venv venv && venv/bin/pip install -r requirements.txt`, then run the notebook from the
repository root.

- `MultiRC/`: the train and test files from the unit's shared folder
- `checkpoints/`: trained weights for every from-scratch model (DistilBERT's is too large and is not included)
- `results/`: `results.csv` (every logged metric), per-epoch training logs (`history_*.csv`), predictions (`preds/`) and the validation split (`splits.json`)
