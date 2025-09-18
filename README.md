# Semantic-Search-Demo-Comparing-TF-IDF-and-Sentence-Embeddings
End-to-end retrieval prototype: TF-IDF vs Sentence-BERT + FAISS on 1 k AG-News articles.

[![Open In Colab](https://colab.research.google.com/drive/1qC-okEYKSKuT5GP13z0ifFt5wB6UHQtC)

## TL;DR
One-click notebook that ingests 1 200 news snippets, builds two search backends (sparse TF-IDF and dense Sentence-BERT + FAISS), evaluates with 10 real queries, and visualizes when sparse beats dense (and vice-versa).

## Key Results
| Metric | TF-IDF | Dense |
|--------|--------|-------|
| Hit@5 | 1.000 | 0.900 |
| MRR | 0.642 | 0.495 |
| Avg latency | 1.2 ms | 6.2 ms |
| Index size | 2 MB | 1.5 MB |

## Stack
Python 3.9 · scikit-learn · sentence-transformers · FAISS · pandas · matplotlib

## Quick Start
```bash
git clone https://github.com/&lt;your-username&gt;/semantic-search-demo.git
cd semantic-search-demo
pip install -r requirements.txt
jupyter notebook semantic_search_demo.ipynb
# Kernel → Restart & Run All
