# 📚 Ask the Paper: A RAG-Based QA System for Research PDFs

A practical Retrieval-Augmented Generation (RAG) pipeline that allows users to ask questions and receive context-aware, document-grounded answers from long research papers in PDF format. This project integrates **FAISS**, **Sentence-Transformers**, **Hugging Face Transformers**, and **LangChain** to build an end-to-end semantic question-answering system.

---

## 🚀 Project Overview

This project demonstrates the power of combining vector-based semantic search with large language models (LLMs) to extract precise information from unstructured long documents.

### 🔍 What it does:
- Parses and splits a research PDF into smaller chunks
- Embeds chunks using a pre-trained transformer model
- Stores embeddings in a FAISS vector store for fast retrieval
- Connects a generative model (`flan-t5-base`) to answer questions grounded in retrieved chunks

---

## 🌍 Real-World Applications

This pipeline has broad applicability across multiple domains where humans interact with complex, dense documents:

| Industry        | Use Case                                                                 |
|----------------|--------------------------------------------------------------------------|
| 🎓 Academia     | Students or researchers asking questions about papers, theses, or books |
| ⚖️ Legal        | Legal assistants querying contracts or case law                         |
| 🏥 Healthcare    | Doctors or analysts querying medical guidelines or clinical PDFs        |
| 🏢 Enterprise    | Employees querying policy documents, reports, or internal knowledge     |

---

## 🛠️ Tech Stack

- **Language Model**: `google/flan-t5-base`
- **Embeddings**: `sentence-transformers/all-MiniLM-L6-v2`
- **Vector Store**: FAISS (via LangChain wrapper)
- **Orchestration**: LangChain
- **Interface**: Google Colab / Jupyter Notebook

---

## 📦 Installation

Clone the repository and open the notebook in Google Colab or Jupyter:

```bash
git clone https://github.com/your-username/ask-the-paper.git
cd ask-the-paper
Install the required libraries (Colab users may skip this)
pip install -U langchain faiss-cpu sentence-transformers transformers
```

---

##🧪 How to Use
1.Upload a PDF file to the notebook.

2.The system splits it into chunks and embeds them.

3.Ask any question related to the PDF content.

4.The RAG system retrieves relevant chunks and generates a grounded answer.

---

##📚 Learnings
 - RAG significantly improves factual accuracy vs standalone LLMs.

 - FAISS allows scalable, semantic retrieval from large corpora.

 - LangChain streamlines end-to-end pipeline construction.

---

## 📜 License
MIT License. See LICENSE file for details.

---

## 🙋‍♂️ Author
Joseph Maina

---
