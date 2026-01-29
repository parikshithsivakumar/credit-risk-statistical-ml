# Team 4 - Home Credit Project

Short project README and setup instructions.

## What to include ✅
- Notebooks: `Team_4_Code.ipynb`
- Scripts and helper modules (if any)
- `requirements.txt` or `environment.yml`
- `README.md`, `LICENSE`

## Data handling ⚠️
- The full dataset is excluded from the repo by default (see `.gitignore`).
- Place the CSV files in `Dataset/` named `application_data.csv` and `previous_application.csv`.
- If the dataset is large, host it externally (Google Drive / Kaggle / S3) and provide a download script.

## Setup (pip)
```bash
python -m venv .venv
.\.venv\Scripts\activate  # Windows
pip install -r requirements.txt
```

## Setup (conda)
```bash
conda env create -f environment.yml
conda activate team4_env
```

## Notes
- The notebook contains some Colab-specific cells (e.g., `google.colab.files.upload()`). Remove or guard those cells if running locally.
- Clear notebook outputs before committing: `jupyter nbconvert --clear-output Team_4_Code.ipynb` or use `nbstripout`.
