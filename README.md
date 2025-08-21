# Biomedical Text Classification using LSTM, GRU and Bahdanau Attention

## Project Overview
This repository contains the implementation and evaluation of deep learning models for biomedical text classification. 
The project utilizes classical machine learning models (SVM, Random Forest) and deep learning architectures (LSTM, GRU) enhanced by Bahdanau attention and various embedding strategies.

## Datasets Used
- **MSKCC Dataset**: Binary classification of genetic mutations (Kaggle challenge).
- **Medical Abstracts Dataset**: Multi-class classification of disease categories (GitHub + Hugging Face).

## Models Implemented
- Classical ML:
  - Linear SVM
  - Random Forest
- Deep Learning (models using word embeddings Glove (300 d) and Fasttext (300d), and BioMedNLP as contextual embeddings):
  - Bidiretional LSTM and GRU (from scratch)
  - Bidiretional LSTM and GRU with GloVe and FastText embeddings
  - Bidiretional LSTM and GRU with Bahdanau Attention
  - Bidiretional LSTM and GRU with BioMedNLP contextual embeddings
    
## 📈 Key Findings
- Bidiretional GRU models outperform bidiretional LSTM in training efficiency and balanced accuracy.
- Class weighting is more effective than SMOTE for handling class imbalance.
- Bidirectional GRU model combined with attention mechanisms using BioMedNLP embeddings show better generalization in few-shot learning scenarios.
