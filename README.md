# DOCUBOT - Local RAG Learning Project

## 📌 Description

DOCUBOT is a local Retrieval-Augmented Generation (RAG) system designed to answer questions based on a set of PDF documents.

The system processes documents, converts them into vector representations, and retrieves relevant context to generate answers using a local large language model (LLM).

This project focuses on data privacy by running entirely on local hardware without relying on external APIs.

---

## ⚠️ Note

This project was built as an experimental exploration of RAG systems.

I used AI tools to assist in building parts of the system, and I am currently working on understanding each component and rebuilding it step by step on my own.

This repository represents my learning process, not a fully self-built production system.

---

## 🧠 What I'm Learning

* How RAG (Retrieval-Augmented Generation) systems work
* Embeddings and vector similarity search
* FastAPI backend development
* Working with local LLMs (Ollama)
* Document processing and chunking strategies

---

## 🛠️ Technologies Used

* Python
* FastAPI
* LangChain
* ChromaDB / FAISS
* Ollama (Llama3, nomic-embed-text)

---

## ⚙️ How It Works

1. PDF documents are loaded and processed
2. Text is split into smaller chunks
3. Each chunk is converted into embeddings
4. Embeddings are stored in a vector database
5. User queries are matched with relevant chunks
6. The LLM generates answers based on retrieved context

---

## 🚀 Setup & Run

```bash
git clone https://github.com/yigitalin/DOCUBOT.git
cd DOCUBOT
pip install -r requirements.txt
```

### Prepare Models

```bash
ollama pull llama3
ollama pull nomic-embed-text
```

### Run Backend

```bash
python -m uvicorn app:app --host 127.0.0.1 --port 8000
```

### Run UI

```bash
streamlit run ui.py
```

---

## 🔮 Future Plans

* Rebuild the system step-by-step without AI assistance
* Improve retrieval accuracy
* Add evaluation metrics
* Optimize chunking and search strategy

---

## 📚 Sample Documents

This project includes example PDF documents related to university processes such as:

* Internship guidelines
* Erasmus programs
* Scholarships
* Graduation requirements

---

## 👤 Author

Yiğit Alın
Computer Engineering Student

---
