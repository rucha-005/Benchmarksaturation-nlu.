# Benchmark Saturation in Natural Language Understanding

This repository contains the code and experimental materials used for the term paper:

**Benchmark Saturation in Natural Language Understanding: Do Human-Level Benchmark Scores Indicate Language Understanding?**

## Overview

This project examines whether strong performance on standard NLU benchmarks necessarily reflects broader language understanding.

A small empirical case study was conducted using the SST-2 sentiment classification task and a pretrained DistilBERT model.

## Model and Dataset

- Dataset: SST-2 validation set
- Validation examples: 872
- Model: `distilbert-base-uncased-finetuned-sst-2-english`
- Library: Hugging Face Transformers

## Evaluation

The model was evaluated on:

1. The complete SST-2 validation set.
2. A simple negation challenge containing positive sentences and their negated versions.
3. A hard linguistic challenge containing examples involving negation, contrast, and complex/compositional sentiment.

## Results

| Evaluation | Accuracy |
|---|---:|
| SST-2 validation | 91.06% |
| Simple positive challenge | 100% |
| Simple negated challenge | 100% |
| Hard linguistic challenge | 70% |

## Repository Files

- `sst2_evaluation.py` – code for running the SST-2 evaluation.
- `negation_challenge_results.csv` – results from the simple negation challenge.
- `hard_linguistic_challenge_results.csv` – examples and results from the hard linguistic challenge.

## Author

Rucha Gajanan Jadhao  
University of Trier  
Summer Semester 2026
