# Credit Card Fraud Detection (Notebook)

A minimal notebook workflow to train a fraud detector on **999 labeled rows** (only 2 positives) and predict on **~1,000,000 unlabeled rows**.

## Files
- `CreditcardFrauddetection.ipynb` — end-to-end training + scoring.

## Data
- **Labeled (train)**: CSV with columns `Amount`, `Time`, `V1..V30`, `Class`.
- **Unlabeled (score)**: CSV with the same columns **except** `Class`.
- Put them in `data/` or update the paths in the notebook.

## Setup
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate
pip install -U pandas numpy scikit-learn imbalanced-learn
