# Fine-tuning DistilBERT for News Classification

## 👥 Team Information

**Course:** Deep Learning  
**Institution:** Telkom University  

| Name | NIM |
| :--- | :--- |
| **Fasya Burhanis Syauqi** | 1103223054 |
| **Muhammad Muhammad Farhan** | 11032320187 |

---

## 🎯 Purpose

This repository contains the implementation of **Task 1: Text Classification**.

The objective is to fine-tune a pre-trained **DistilBERT** model to automatically categorize news articles into specific topics. Given a headline and description, the model predicts the correct category.

## 🔍 Project Overview

### The Task: Single-Label Classification
We aim to classify news articles into one of four mutually exclusive categories. This is a fundamental NLP task useful for content organization and recommendation systems.

### The Model: DistilBERT Base Uncased
* **Architecture:** Distilled version of BERT (Transformer Encoder).
* **Approach:** We use the `[CLS]` token output passed through a classification layer to predict the probability of each class.

### The Dataset: AG News
* **Input:** Text containing the news title and description.
* **Output:** One of 4 categories:
  * 0: World
  * 1: Sports
  * 2: Business
  * 3: Sci/Tech

---

## 📊 Technical Approach

### Model Configuration
* **Base Model:** `distilbert-base-uncased`
* **Tokenizer:** DistilBertTokenizer
* **Framework:** PyTorch & Hugging Face Transformers

### Training Configuration
* **Batch Size:** 64
* **Learning Rate:** 2e-5
* **Epochs:** 3
* **Optimizer:** AdamW

### Results
The model achieved an accuracy of approximately **94.8%** on the test set.

---

## 📁 Repository Structure

```text
project_agnews/
│
├── notebooks/
│   └── Task1_AGNews.ipynb    # Main Jupyter Notebook for Training
│
├── reports/
│   └── report.md             # Training results and analysis
│
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
