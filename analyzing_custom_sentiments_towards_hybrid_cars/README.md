# Hybrid Car Sentiment Analysis

A machine learning project that analyzes consumer sentiment towards hybrid cars in India using online reviews.

## Overview

This project processes 2,000 customer reviews collected from Indian hybrid car review websites and classifies them as positive or negative using Naïve Bayes and Support Vector Machine (SVM) models. Word frequency analysis is used to identify key themes driving consumer perception.

## Project Structure

```
├── Hybrid_Car_Sentiment_Analysis.ipynb   # Main notebook
├── Hybrid_Car_Reviews.xlsx               # Dataset
└── README.md
```

## Dataset

- 2,000 reviews from Indian hybrid car review websites
- 3 columns: `Review`, `Ratings` (1–5), `Rating style` (Positive/Negative)
- ~89% Positive, ~11% Negative reviews

## Methods

- **Pre-processing** — lowercasing, special character removal, stopword filtering, stemming
- **Vectorization** — TF-IDF (unigrams + bigrams)
- **Models** — Naïve Bayes and Support Vector Machine (SVM)
- **Evaluation** — Accuracy, Precision, Recall, F1-Score, Confusion Matrix, Sensitivity & Specificity

## Results

| Model | Accuracy |
|-------|----------|
| Naïve Bayes | ~90.4% |
| SVM | ~90.6% |

## Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl ipywidgets
```

## Usage

1. Clone the repository
2. Place `Hybrid_Car_Reviews.xlsx` in the same folder as the notebook
3. Install dependencies using the command above
4. Run `Hybrid_Car_Sentiment_Analysis.ipynb` cell by cell

## Reference

> Full research paper available [here](https://link.springer.com/chapter/10.1007/978-981-97-8602-2_40).