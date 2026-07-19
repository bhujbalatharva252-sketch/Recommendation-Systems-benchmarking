# Recommendation Systems Benchmarking Using Traditional Models and Large Language Models

## Project Overview

This project investigates and compares traditional recommendation system approaches with Large Language Model (LLM)-based recommendation approaches using a unified evaluation framework.

The objective is to evaluate whether LLMs can perform competitive recommendation tasks compared with conventional recommendation algorithms under the same evaluation conditions.

---

## Dataset

Dataset used:

**MovieLens 1M Dataset**

The dataset contains:
- User ratings
- Movie metadata
- User information

Data preprocessing includes:
- Rating data cleaning
- Train/test splitting
- Candidate set generation

---

## Evaluation Framework

A unified candidate-based evaluation framework is used for all models.

For each user:
- 1 positive test item
- 99 negative candidate items

Each model ranks the same candidate set.

Evaluation metrics:

- Hit@10
- NDCG@10

This ensures a fair comparison between traditional recommendation models and LLM-based approaches.

---

## Implemented Models

### Traditional Recommendation Models

1. Popularity Baseline
2. Content-Based Filtering (TF-IDF)
3. SVD Collaborative Filtering


### LLM-Based Recommendation Models

1. Mistral-7B-Instruct
2. Gemma-7B-Instruct
3. Llama-3.1-8B-Instruct

LLMs are prompted to rank candidate movies based on the user's historical preferences.

---
