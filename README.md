# Semantic Search Engine: TF-IDF vs. Sentence Transformers

[![Open in Colab](https://colab.research.google.com/drive/1qC-okEYKSKuT5GP13z0ifFt5wB6UHQtC)
[![GitHub](https://img.shields.io/badge/GitHub-Repo-black?style=flat&logo=github)](https://github.com/your-username/your-repo-name)

A comparative analysis of traditional sparse (TF-IDF) and modern dense (Sentence-BERT) retrieval methods implemented in Python. This project demonstrates the strengths and weaknesses of each approach on the AG News dataset with comprehensive evaluation metrics.

## 📖 Project Overview

This project implements a complete semantic search pipeline comparing:
1. **TF-IDF Retrieval**: Traditional sparse vector approach using scikit-learn
2. **Dense Embeddings**: Neural semantic search using Sentence-BERT and FAISS

The system processes 1,200+ news articles, handles natural language queries, and provides side-by-side comparison of top results from both methods.

## 🚀 Features

- **Dual Retrieval Systems**: TF-IDF with scikit-learn + Sentence-BERT with FAISS
- **Comprehensive Evaluation**: 10 test queries with Hit@K and MRR metrics
- **Visual Analytics**: Comparative performance charts and results visualization
- **Error Analysis**: Detailed breakdown of when each method succeeds/fails
- **Production Ready**: Clean, modular code with proper documentation

## 📊 Results Summary

| Model | Hit@1 | Hit@5 | MRR | Avg. Query Time |
| :--- | :---: | :---: | :---: | :---: |
| **TF-IDF** | 0.400 | 1.000 | 0.842 | ~1.2 ms |
| **Dense Embeddings** | 0.300 | 0.800 | 0.495 | ~6.2 ms |

### Key Insights:
- ✅ **TF-IDF excels** at keyword-heavy queries (e.g., "Olympic games athletes medals")
- ✅ **Dense Embeddings excel** at semantic queries (e.g., "How to manage company finances?")
- ⚡ **TF-IDF is 5x faster** for query processing
- 🎯 **Dense embeddings** provide better semantic understanding

## 🛠️ Installation & Usage

```bash
# Clone repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run in Jupyter notebook or Google Colab
jupyter notebook semantic_search_comparison.ipynb
