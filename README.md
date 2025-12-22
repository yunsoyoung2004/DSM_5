
# DSM-5 Based Multi-label Depression Detection

This repository contains the Jupyter notebooks used in the study:

**“Leveraging DSM-5 for Advanced Depression Detection:  
A Comprehensive Study on Korean Speech and Text Data”**

The goal of this study is to detect depressive symptoms by performing
multi-label classification based on nine DSM-5 diagnostic criteria
using multiple NLP models.

---

## Overview

We implemented and evaluated four models:

- Word2Vec (W2V)
- Seeded LDA
- Paragraph Vector (PV / Doc2Vec)
- KoBERT

Each model performs multi-label classification corresponding to
nine DSM-5 depressive disorder criteria.
Model performance was evaluated using weighted, macro, and micro F1-scores.

All experiments are provided as **Jupyter notebooks** to improve
readability and transparency of the experimental pipeline.

---

## Repository Structure

```text
DSM5-Depression-Detection/
 ├─ README.md
 ├─ requirements.txt
 ├─ notebooks/
 │   ├─ 01_data_format_description.ipynb
 │   ├─ 02_labeling_rules_DSM5.ipynb
 │   ├─ 03_train_w2v.ipynb
 │   ├─ 04_train_seeded_lda.ipynb
 │   ├─ 05_train_pv.ipynb
 │   ├─ 06_train_kobert.ipynb
 │   └─ 07_evaluation_metrics.ipynb
 └─ data/
     └─ README.md
