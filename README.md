# 🚀 NL2SQL with RAG

A Retrieval-Augmented Generation (RAG) based Natural Language to SQL system that converts user questions into SQL queries using semantic schema retrieval.

## 📌 Overview

This project improves SQL generation by retrieving the most relevant database schemas before query generation. Instead of processing the entire database schema, the system uses vector embeddings and semantic search to provide only the necessary context to the language model.

## ✨ Features

- Natural Language to SQL (NL2SQL)
- Retrieval-Augmented Generation (RAG)
- Semantic Schema Search
- FAISS Vector Similarity Search
- Sentence Transformer Embeddings
- Spider Dataset Integration
- LoRA Fine-Tuned BART Model

## 🛠️ Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- Sentence Transformers
- FAISS
- Streamlit
- Spider Dataset

## ⚙️ Workflow

```text
User Query
    ↓
Schema Retrieval
    ↓
Vector Similarity Search
    ↓
Relevant Tables
    ↓
Context Generation
    ↓
SQL Generation
```

## 📂 Project Structure

```text
nl2sql_demo/
├── main.py
├── nl2sqlSchemas.py
├── requirements.txt
├── spider/
└── bart_large_lora_spider/
```

## 🎯 Example

**Input:**
```text
Show students with CGPA greater than 8.5
```

**Generated SQL:**
```sql
SELECT * FROM Student
WHERE cgpa > 8.5;
```

## 🚀 Run Locally

```bash
pip install -r requirements.txt
python main.py
```

## 👨‍💻 Author

**Eshwar Kumar**

