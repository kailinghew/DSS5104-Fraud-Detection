# DSS5104 Fraud Detection Assignment

This project runs a Jupyter notebook for fraud and anomaly detection using:
- IEEE-CIS Fraud Detection data
- Credit Card Fraud data

## Project Structure

Keep this structure unchanged so file paths in the notebook work:

```text
DSS5104 Assignment/
  DSS5104_hewkailing.ipynb
  requirements.txt
  creditcardfraud/
    creditcard.csv
  ieee-fraud-detection/
    train_transaction.csv
    train_identity.csv
    test_transaction.csv
    test_identity.csv
    sample_submission.csv
```

  ## Download Datasets

  You can download the datasets from Kaggle:

  - IEEE-CIS Fraud Detection: https://www.kaggle.com/c/ieee-fraud-detection
  - Credit Card Fraud Detection: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

  After downloading:

  1. Place the IEEE-CIS CSV files in `ieee-fraud-detection/`:
     - `train_transaction.csv`
     - `train_identity.csv`
     - `test_transaction.csv`
     - `test_identity.csv`
  2. Place `creditcard.csv` in `creditcardfraud/`.

## 1. Create and Activate a Python Environment

### Windows (PowerShell)
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### macOS/Linux (bash/zsh)
```bash
python3 -m venv .venv
source .venv/bin/activate
```

## 2. Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

## 3. Launch Jupyter

From the project root (`DSS5104 Assignment`):

```bash
jupyter notebook
```

Then open:
- `DSS5104_hewkailing.ipynb`

## 4. Run the Notebook

1. Select the Python kernel from your `.venv` environment.
2. Run cells from top to bottom (`Run All` is recommended).
3. Wait for training and evaluation cells to finish; some models may take longer.

## Notes

- The notebook uses relative paths such as:
  - `ieee-fraud-detection/train_transaction.csv`
  - `creditcardfraud/creditcard.csv`
- If you move the notebook or data folders, update paths in the notebook accordingly.

## Troubleshooting

### `ModuleNotFoundError`
Re-activate your environment and reinstall requirements:

```bash
pip install -r requirements.txt
```

### Wrong kernel in notebook
Switch kernel in Jupyter/VS Code to the one inside `.venv`.

### File not found errors
Make sure you are running Jupyter from the project root and data folders exist exactly as listed above.
