# 🌟 VibeMatcher — AI-Powered Fashion Recommender by Nexora

> **"Find your fashion vibe — powered by AI."**

VibeMatcher is a mini AI-based recommendation system that matches short *“vibe”* queries (like **“energetic urban chic”**) with the most relevant fashion products using OpenAI embeddings and cosine similarity.  
It blends semantic understanding with product metadata (tags, popularity, tone) to make recommendations that *feel right*, not just *look right*.

---

## ✨ Features
- 🧠 **AI Semantic Matching:** Uses `text-embedding-ada-002` from OpenAI for deep vibe understanding  
- 🎯 **Smart Ranking:** Combines embedding similarity + tag overlap + popularity weighting  
- ⚡ **Fast Retrieval:** Cosine similarity via scikit-learn  
- 💬 **Fallback Handling:** Gracefully suggests similar vibes when no confident match found  
- 📊 **Evaluation Metrics:** Precision@K, MRR, Average Top Score, Latency plots  
- 🔁 **Reproducible & Modular:** Seeded, clean, and Colab-ready notebook  

---

## 🧩 Project Overview

| Task Component | Description |
|----------------|--------------|
| **Goal** | Build a vibe-based mini recommendation engine |
| **Embedding Model** | `text-embedding-ada-002` (OpenAI API) |
| **Similarity Metric** | Cosine Similarity (`sklearn`) |
| **Dataset** | 8 mock fashion products with descriptions + tags |
| **Evaluation** | 3 queries → similarity scores, latency, and metrics |
| **Threshold** | 0.7 for “good” similarity |
| **Results** | Precision@1 = 1.0 • MRR = 1.0 • Avg Score = 0.83 |

---

## 🚀 How to Run in Google Colab

1. Open the notebook **`SanskarNexoratask.ipynb`** in [Google Colab](https://colab.research.google.com/).  
2. Install dependencies:
   ```python
   !pip install openai pandas numpy scikit-learn matplotlib
