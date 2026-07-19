# Deep Learning Research Internship — Final Project (SS 2026)

Applied deep learning projects completed as the final task of a graded research
internship (*Forschungspraktikum Deep Learning*) at the **Institute for Computer
Science, University of Koblenz**, supervised by Jennifer Wendland and
Prof. Dr. Maik Kschischo.

**Final internship grade: 1.0 (with distinction).**

The final task moves beyond textbook exercises into two self-contained applied
projects: a clinical classification pipeline and a multi-domain time-series
forecasting study.

> **Declaration of AI usage:** These notebooks were developed with the assistance
> of generative AI tools for concept study, code development/debugging, and
> presentation. All experiments, model choices, evaluation, and analysis were
> designed, run, and interpreted by me. Each notebook contains a full AI-usage
> declaration.

---

## Task 1 — Heart Disease Prediction (Feed-Forward Neural Network)

A complete binary-classification pipeline in PyTorch predicting the presence of
heart disease from clinical features.

**What it covers**
- Data cleaning and one-hot encoding of categorical clinical features
- Stratified train / validation / test split with feature scaling
- Feed-forward network (PyTorch `Sequential`, Adam optimizer)
- Training loop with **early stopping** and loss/accuracy curve visualization
- Evaluation: test-set metrics, **decision-threshold tuning**, **ROC curve**, and
  confusion matrix
- A **hyperparameter study** across model configurations

**Files:** `Heart_Disease_Prediction_with_a_Feed-Forward_Neural_Network.ipynb`,
`heart.csv`

---

## Task 2 — Time-Series Forecasting (GRU)

Recurrent forecasting applied to three progressively harder systems — real-world,
chaotic, and biological — using a GRU-based model.

**Part A — Delhi Weather (real data)**
Windowed forecasting of daily temperature from the Daily Delhi Climate dataset;
train/test evaluation and forecast visualization.

**Part B — Lorenz System (chaotic dynamics)**
Simulating the Lorenz attractor and training a model to roll out forecasts of a
chaotic system — testing how far ahead a neural forecaster can track divergence.

**Part C — Synthetic Tumour Growth (biological dynamics)**
A custom tumour-growth simulator generating data, with a model trained to predict
growth trajectories.

**Files:** `Time_Series_Forecasting.ipynb`, `DailyDelhiClimateTrain.csv`,
`DailyDelhiClimateTest.csv`

---

## Tech stack

`Python` · `PyTorch` · `NumPy` · `Pandas` · `scikit-learn` · `Matplotlib`

## Reproducibility

Each notebook sets random seeds and documents its preprocessing, so results can be
reproduced end-to-end. Datasets are included in the repository.

---

## About the internship

The full internship followed the *Dive into Deep Learning* (Zhang et al.)
curriculum across MLPs, CNNs, and RNNs, with weekly exercises building up to this
final applied project. This repository contains the **final task**; it is the
capstone of the graded internship.
