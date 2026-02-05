# Natural Language Processing - University of Bologna

This repository contains assignments and projects completed for the Natural Language Processing course at the University of Bologna (Unibo). The work includes implementations of various NLP tasks such as Part-of-Speech (POS) tagging, claim verification, question answering, and keyword extraction using state-of-the-art neural architectures.

## 📚 Table of Contents

- [Overview](#overview)
- [Repository Structure](#repository-structure)
- [Assignments](#assignments)
  - [Assignment 1: POS Tagging](#assignment-1-pos-tagging)
  - [Assignment 2: Claim Verification](#assignment-2-claim-verification)
- [Projects](#projects)
  - [Question Answering System](#question-answering-system)
  - [Pipeline Extension](#pipeline-extension)
- [Installation](#installation)
- [Usage](#usage)
- [Authors](#authors)
- [License](#license)

## 🎯 Overview

This repository showcases comprehensive work in Natural Language Processing, implementing various neural architectures and techniques to solve real-world NLP problems. The projects leverage modern deep learning frameworks and pre-trained models including BERT, DistilBERT, RoBERTa, and ALBERT.

## 📁 Repository Structure

```
.
├── Assignments/
│   ├── Assignment_1/          # POS Tagging with RNNs
│   │   ├── assignment_1.ipynb
│   │   └── dependency_treebank/
│   └── Assignment_2/          # Claim Verification
│       ├── Assignment_2.ipynb
│       ├── README.md
│       └── dataset/
├── Project/                   # Question Answering System
│   ├── NLP_Project_Aspromonte_Boriano_Morselli_Romito.ipynb
│   ├── NLP_report_Aspromonte_Boriano_Morselli_Romito.pdf
│   ├── README.md
│   ├── evaluate.py
│   ├── evaluation_custom.py
│   └── test_duorc.json
├── Pipeline_Romito_Aspromonte.ipynb  # Keyword Extraction Pipeline
├── NLP_extention_report.pdf
├── natural_questions_500.csv
└── train_dbpedia.json
```

## 📝 Assignments

### Assignment 1: POS Tagging

**Objective**: Implement Part-of-Speech tagging using Recurrent Neural Networks (RNNs) as a sequence labeling task.

**Key Features**:
- Dataset: NLTK Dependency Treebank corpus
- Embeddings: Pre-trained GloVe word embeddings
- Architectures: Bidirectional LSTM and GRU models
- Evaluation: F1-Macro score (excluding punctuation classes)
- Data Split: Documents 1-100 (train), 101-150 (validation), 151-199 (test)

**Highlights**:
- Proper handling of Out-of-Vocabulary (OOV) terms
- Multiple architecture experiments (LSTM, GRU, multi-layer variants)
- Comprehensive error analysis and performance evaluation

**Location**: `Assignments/Assignment_1/assignment_1.ipynb`

### Assignment 2: Claim Verification

**Objective**: Develop a system to verify claims against supporting or refuting evidence using deep learning approaches.

**Key Features**:
- Multi-input classification with sentence embeddings
- Dataset cleaning and preprocessing
- Various embedding strategies for claims and evidence
- Neural network architectures for classification

**Highlights**:
- Structured implementation with clean separation of code and specifications
- Focus on dataset quality and preprocessing

**Location**: `Assignments/Assignment_2/Assignment_2.ipynb`

## 🚀 Projects

### Question Answering System

**Objective**: Build a Question Answering system trained on the SQuAD dataset and evaluated on both SQuAD and DuoRC datasets.

**Team**: Marco Aspromonte, Valentina Boriano, Enrico Morselli, Francesco Romito

**Key Features**:
- Dataset: SQuAD (Stanford Question Answering Dataset)
- Models: DistilBERT, DistilRoBERTa, ALBERT v2
- Train/Validation Split: 75%/25% of SQuAD dataset
- Optional test on DuoRC dataset for cross-dataset evaluation

**Implementation Details**:
- Fine-tuning of pre-trained transformer models
- Custom evaluation metrics
- Support for multiple model variants
- Pre-trained model weights available via Google Drive

**Files**:
- Main notebook: `Project/NLP_Project_Aspromonte_Boriano_Morselli_Romito.ipynb`
- Detailed report: `Project/NLP_report_Aspromonte_Boriano_Morselli_Romito.pdf`
- Evaluation script: `Project/evaluation_custom.py`

**Pre-trained Weights**: Available at [Google Drive Link](https://drive.google.com/file/d/1D-vLDgUjXwbFs0honajJaPF-iMHP5Yga/view)

### Pipeline Extension

**Objective**: Extend the Question Answering system with keyword extraction capabilities evaluated on DBpedia.

**Authors**: Francesco Romito, Marco Aspromonte

**Key Features**:
- Keyword extraction models
- Evaluation using DBpedia dataset
- Integration with the main QA pipeline
- Comprehensive performance metrics

**Files**:
- Main notebook: `Pipeline_Romito_Aspromonte.ipynb`
- Extension report: `NLP_extention_report.pdf`

## 🛠️ Installation

### Prerequisites

- Python 3.7+
- Jupyter Notebook or JupyterLab
- pip or conda package manager

### Required Libraries

```bash
# Core libraries
pip install numpy pandas matplotlib

# NLP and Deep Learning
pip install torch transformers
pip install tensorflow keras  # Alternative framework

# Utilities
pip install nltk scikit-learn
```

### Additional Setup

For Assignment 1, download GloVe embeddings:
```bash
# Download GloVe embeddings (e.g., glove.6B.100d.txt)
wget http://nlp.stanford.edu/data/glove.6B.zip
unzip glove.6B.zip
```

## 💻 Usage

### Running Assignments

1. **Assignment 1 - POS Tagging**:
   ```bash
   cd Assignments/Assignment_1
   jupyter notebook assignment_1.ipynb
   ```

2. **Assignment 2 - Claim Verification**:
   ```bash
   cd Assignments/Assignment_2
   jupyter notebook Assignment_2.ipynb
   ```

### Running Projects

1. **Question Answering System**:
   ```bash
   cd Project
   jupyter notebook NLP_Project_Aspromonte_Boriano_Morselli_Romito.ipynb
   ```
   
   Follow the instructions in the notebook to:
   - Choose between SQuAD validation set or DuoRC as test set
   - Select model variant (DistilBERT, DistilRoBERTa, or ALBERT)
   - Train or load pre-trained weights

2. **Pipeline Extension**:
   ```bash
   jupyter notebook Pipeline_Romito_Aspromonte.ipynb
   ```

## 👥 Authors

### Question Answering Project
- Marco Aspromonte
- Valentina Boriano
- Enrico Morselli
- Francesco Romito

### Pipeline Extension
- Francesco Romito
- Marco Aspromonte

## 📄 License

This project is part of academic coursework at the University of Bologna. All rights reserved by the respective authors.

## 🙏 Acknowledgments

- **Course Instructors**: Prof. Paolo Torroni
- **Teaching Assistants**: Andrea Galassi, Federico Ruggeri
- **Institution**: University of Bologna (Unibo)
- **Datasets**: SQuAD, DuoRC, DBpedia, NLTK Dependency Treebank

---

*This repository represents coursework completed for the Natural Language Processing course at the University of Bologna.*