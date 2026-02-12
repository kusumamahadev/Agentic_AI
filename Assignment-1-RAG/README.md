# 📈 FinRAG-Analyst: Automated Financial Insight Engine

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://agentic-ai-kp49jrq34o2aodammy8w2s.streamlit.app/)

> **Assignment 1: Retrieval-Augmented Generation (RAG) System**
> *Analyzes the Apple 2025 10-K Financial Report using Llama 3 & Vector Search.*

---

## 🚀 Project Overview
**FinRAG-Analyst** (codenamed "Project Nucleus") is an AI-powered financial research tool designed to answer complex queries about SEC 10-K filings. 

Unlike standard LLMs, this system uses a **RAG (Retrieval-Augmented Generation)** architecture to fetch real-time evidence from the document before answering. This ensures **zero hallucination** and provides accurate, citation-backed insights for financial analysts.

### 🌟 Key Features
* **Zero-Hallucination Mode:** Uses `temperature=0` to ensure strict factual accuracy.
* **Source Citations:** Retrieves and references specific chunks from the 10-K PDF.
* **Hybrid Architecture:** Decoupled **FastAPI** backend and **Streamlit** frontend.
* **Vector Search:** Powered by **ChromaDB** and **HuggingFace Embeddings**.

---

## 🛠️ Tech Stack
| Component | Technology | Description |
| :--- | :--- | :--- |
| **LLM** | **Llama 3.3-70b** | High-speed inference via **Groq API** |
| **Orchestration** | **LangChain** | Manages the RAG pipeline |
| **Database** | **ChromaDB** | Stores vector embeddings |
| **Backend** | **FastAPI** | High-performance API server |
| **Frontend** | **Streamlit** | Interactive chat interface |

---

## 📂 Project Structure
```text
Assignment-1-RAG/
├── api/                # FastAPI Backend
│   └── server.py       # API Endpoints
├── core/               # AI Engine (The Brain)
│   ├── ingest.py       # PDF Loader & Vectorization
│   └── rag.py          # RAG Retrieval Chain
├── ui/                 # Frontend Interface
│   └── app.py          # Streamlit Chat Dashboard
├── data/               # Raw Data
│   └── apple_2025_10k.pdf
├── vectorstore/        # Pre-computed Vector Database
├── notebooks/          # Lab Experiments
│   └── RAG_Demonstration.ipynb
├── requirements.txt    # Python Dependencies
└── streamlit_app.py    # Cloud Deployment Script
⚡ Installation & Setup
1. Clone the Repository
Bash
git clone [https://github.com/theMeghna/Agentic-AI.git](https://github.com/theMeghna/Agentic-AI.git)
cd "Agentic-AI/Assignment-1-RAG"
2. Create a Virtual Environment
Bash
python -m venv venv
# Windows
.\venv\Scripts\activate
# Mac/Linux
source venv/bin/activate
3. Install Dependencies
Bash
pip install -r requirements.txt
4. Configure Environment Keys
Create a .env file in the root directory and add your Groq API Key:

Ini, TOML
GROQ_API_KEY=gsk_your_actual_key_here
🏃‍♂️ How to Run Locally
Open two separate terminals:

Terminal 1: Start the Backend API

Bash
python api/server.py
Terminal 2: Start the Frontend UI

Bash
streamlit run ui/app.py
🧪 Testing & Verification
We have included a Jupyter Notebook to verify the RAG logic step-by-step:

Open notebooks/RAG_Demonstration.ipynb

Run all cells to see the Ingestion -> Retrieval -> Generation process in action.

👥 Team Members
Meghna Sahu - Team Lead & AI Engineer

Kusuma - Frontend Developer

Harshit Sangwan - Backend Developer
