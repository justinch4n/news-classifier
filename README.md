# News Classifier

End-to-end fake-news classification project with interpretable baselines and neural models.

## What this repo includes
- EDA and data quality checks
- Time-based train/test split
- Full-text TF-IDF + Logistic Regression baseline
- Full-text DistilBERT fine-tuning
- DANN (domain-adversarial) experiment
- Headline-only TF-IDF baseline
- Headline-only DistilBERT and headline-only DANN experiments

## Dataset Citation
Clément Bisaillon. *Fake and Real News Dataset*. Kaggle.
https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset/data

## Files
- `Fake_News_End_to_End.ipynb` — main notebook
- `requirements.txt` — Python dependencies

## Quick Start (Local)
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook Fake_News_End_to_End.ipynb
```

## Quick Start (Google Colab)
1. Upload notebook and dataset files (`Fake.csv`, `True.csv`).
2. Place dataset files in `sample_data/` or `data/`.
3. Run notebook top-to-bottom.

## Notes
- DistilBERT gives top performance but takes significantly longer to train.
- TF-IDF baseline is much faster and still strong.
