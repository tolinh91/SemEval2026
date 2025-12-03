# ⚖️ SemEval-2026 - Task 12

## 📋 Mục lục

- [Introduction](#introduction)
- [System Requirement](#system-requirements)
- [Configuration](#configuration)
- [Folder Structure](#folder-structure)
- [Contributors](#contribution)
- [License](#license)

##  Introduction

This repository contains the code and system description for Team UIT-Goodguys, developed for SemEval 2026 Task 12.
Our submission employs a BERT backbone combined with Retrieval-Augmented Generation (RAG) and lightweight reasoning mechanisms to improve contextual understanding and classification accuracy.

The goal of the task is to (briefly describe the task — optional; fill in later if task description is announced).

## 🚀 System Summary
🔧 Model Backbone: BERT (base uncased)

Used for both: Embedding text segments

Downstream classification via fine-tuning

## 🧩 Key Techniques

RAG (Retrieval-Augmented Generation)
Retrieval is used to enrich the context fed into the model.

Lightweight Reasoning Module
Simple chain-of-thought–style prompting and structured intermediate reasoning to improve prediction stability.

## 🛠 Preprocessing & Post-processing

No special preprocessing

No additional post-processing beyond model output

## 🏗 Frameworks

PyTorch (via HuggingFace Transformers abstraction)

transformers library (HuggingFace)

### Reposity Structure
├── data/
│   ├── train/
│   ├── dev/
│   └── test/
├── src/
│   ├── dataset.py
│   ├── SemEval2026-chunking.py
│   ├── SemEval2026-Embedding.py
│   ├── reasoning.py
│   └── train.py
├── outputs/
│   └── predictions.json
├── README.md
└── requirements.txt

## 🚀 Configuration

### 1. Clone repository

```bash
git clone <repository-url>
cd SemEval2026
```

### 2. Virtual Environment (recomend)

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**Linux/Mac:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Dependencies Configuration

```bash
pip install -r requirements.txt
```

### 4. Data Preparation
Add dataset to data folder.
```
data/
  ├── faq.csv          # File FAQ (question, answer, category)
  ├── laws/            # Thư mục chứa văn bản pháp luật
  └── ...
```

## Results
| Metric   | Score         |
| -------- | ------------- |
| Accuracy | *To be added* |
| F1-score | *To be added* |
| Ranking  | *To be added* |


## 📄 Liencese
This project is released under the MIT License.

## 👥 Contributors

**UIT Goodguys**
1. Linh Thi To Tran
2. Tung Hoang
3. Duy Pham The Ngo
4. Manh Van Le

## Citation
@misc{uitgoodguys2026semeval12,
  title = {UIT-Goodguys at SemEval 2026 Task 12: BERT-based Retrieval-Augmented Reasoning},
  author = {UIT-Goodguys Team},
  year = {2026},
  note = {SemEval 2026 Task 12}
}






