# 🧪 LLM & Multimodal AI Implementation Lab

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red.svg)
![HuggingFace](https://img.shields.io/badge/HuggingFace-Transformers-yellow.svg)
![RAG](https://img.shields.io/badge/RAG-LLM%20Pipelines-green.svg)
![Multimodal](https://img.shields.io/badge/Multimodal-AI-purple.svg)

Welcome to the **AI Implementation Lab** — a hands-on repository exploring two of the most powerful frontiers in modern AI:

🚀 Retrieval-Augmented Generation (RAG) with optimal data engineering  
🖼️ Vision-Language Multimodal Learning with fine-tuned models  

This lab bridges the gap between **AI demos** and **production-grade systems**.

---

## 🧠 What’s Inside

### 📚 1. The 5 Levels of Text Splitting for RAG

Master chunking strategies that dramatically impact retrieval quality and LLM performance.

| Level | Strategy | Best Use Case |
|------|---------|-------------|
| 01 | Character Splitting | Small docs, quick testing |
| 02 | Recursive Splitting | General-purpose RAG |
| 03 | Document Specific | Code & Markdown handling |
| 04 | Semantic Splitting | Topic-aware chunking |
| 05 | Agentic Splitting | LLM-driven dynamic chunks |

📌 File: `5_Levels_Of-Text_Splitting.ipynb`

---

### 🖼️ 2. Fine-Tuning BLIP (Vision + Language)

Train AI models to understand images with domain-specific captions.

**Highlights:**
- Pretrained Model: BLIP (Bootstrapping Language-Image Pre-training)
- Dataset: `ybelkada/football-dataset`
- Framework: PyTorch + Hugging Face

**Key Learnings:**
✔ Custom dataset pipelines  
✔ Multimodal processors  
✔ Gradient-based fine-tuning  

📌 File: `Fine_tune-BLIP.ipynb`

---

## 📂 Project Structure

```bash
Advanced-AI-Lab/
│
├── notebooks/
│   ├── 5_Levels_Of-Text_Splitting.ipynb
│   └── Fine_tune-BLIP.ipynb
│
├── data/
│   └── sample_datasets/
│
├── requirements.txt
├── README.md
└── .gitignore

🛠️ Installation
git clone https://github.com/YourUsername/Advanced-AI-Lab.git
cd Advanced-AI-Lab
pip install -r requirements.txt
