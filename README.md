# Seizure Prediction Using Hybrid CNN-TCN Model

A deep learning model for epileptic seizure prediction using EEG signals from the CHB-MIT Scalp EEG Database.

## Published Paper

This work is published in IEEE:
"Hybrid CNN-TCN Modeling of EEG Temporal Signals for Epileptic Seizure Prediction"
https://ieeexplore.ieee.org/document/11159432/

## Overview

Epilepsy affects over 50 million people worldwide. Sudden seizures pose serious risks to patients' safety. This project proposes a hybrid CNN-TCN architecture to classify ictal and pre-ictal EEG segments, enabling early seizure prediction.

## Dataset

CHB-MIT Scalp EEG Database (pediatric patients), preprocessed with ictal and pre-ictal labels.

## Model Architecture

- CNN Block: spatial feature extraction with Conv1D, BatchNorm, MaxPooling, Dropout
- TCN Block: temporal pattern modeling with dilated causal convolutions
- Elastic Net regularization (L1 + L2) to reduce overfitting
- 10-fold cross-validation

## Results

| Metric | Score |
|--------|-------|
| Accuracy | 99.49% |
| ROC AUC | 1.00 |

Outperformed baseline models: CNN, LSTM, and LSTM-TCN.

## Tech Stack

Python, TensorFlow, Keras, NumPy, Pandas, scikit-learn, Matplotlib, Seaborn

## Authors

Yara Alotaibi, Mashael Al-Luhaybi, Joud Alharbi, Bushra Majrashi, Zulfa Alharbi, Maryam Alhindi

Umm Al-Qura University, Mecca, Saudi Arabia
