# DSM-5 Based Multi-label Depression Detection

This repository contains the source code and Jupyter notebooks used in the study:

**“Leveraging DSM-5 for Advanced Depression Detection:  
A Comprehensive Study on Korean Speech and Text Data”**

This study aims to detect depressive symptoms by performing multi-label
classification based on the nine diagnostic criteria of depressive
episodes defined in the DSM-5, using multiple natural language processing
(NLP) models.

---

## Overview

We implemented and evaluated the following four models:

- Word2Vec (W2V)
- Seeded Latent Dirichlet Allocation (Seeded LDA)
- Paragraph Vector (PV / Doc2Vec)
- KoBERT

Each model performs multi-label classification corresponding to the
nine DSM-5 diagnostic criteria for depressive disorder.
Model performance was evaluated using weighted, macro, and micro
F1-scores on two datasets (wellness data and Everytime data).

All experiments are provided as **Jupyter notebooks** to improve
readability, transparency, and reproducibility of the experimental
pipeline.

---

## Repository Structure

```
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
```

---
Data Availability
Due to legal and ethical restrictions, the original Everytime dataset
cannot be shared publicly.
The wellness dataset was used under license and therefore cannot be
redistributed.

To support transparency and reproducibility, this repository provides:

Complete source code for preprocessing, training, and evaluation

Execution scripts and notebooks corresponding to all experiments

Synthetic sample data that replicate the structure of the original data
without containing identifiable or proprietary information

Further details regarding data restrictions are described in the
data/README.md file.

---

Reproducibility
All experiments were conducted using fixed random seeds to ensure
reproducibility.
The notebooks are organized to reproduce the experimental results
reported in the paper, including:

Data formatting and labeling rules based on DSM-5 criteria

---

Model training procedures

Evaluation using weighted, macro, and micro F1-scores

By following the notebook order, users can reproduce the experimental
pipeline described in the manuscript.

Requirements
Python 3.9 or later

PyTorch

HuggingFace Transformers

KoBERT dependencies

Additional Python packages listed in requirements.txt

---

How to Run
Install dependencies:

pip install -r requirements.txt
Launch Jupyter Notebook and run the notebooks in order:

01_data_format_description.ipynb

02_labeling_rules_DSM5.ipynb

03_train_w2v.ipynb

04_train_seeded_lda.ipynb

05_train_pv.ipynb

06_train_kobert.ipynb

07_evaluation_metrics.ipynb

Each notebook corresponds to a specific stage of the experimental
pipeline described in the paper.

---

License
This project is released under the MIT License.
See the LICENSE file for details.
