# 📄 Document Question Answering AI Agent (Gemini + RAG)

This project implements a **Document Question Answering AI Agent** that allows users to upload multiple documents (PDFs) and ask natural language questions about their content.  
The system uses a **Retrieval-Augmented Generation (RAG)** approach, combining vector-based document retrieval with **Google Gemini API** for accurate, context-aware answers.

This project was developed as part of a **Junior AI Engineer Competency Assessment**.

---


## 🚀 Key Features

- Upload and process multiple PDF documents  
- Automatic text extraction and chunking  
- Local embedding generation to avoid API rate limits  
- Fast semantic search using FAISS vector database  
- Context-aware question answering using **Gemini Flash model**  
- End-to-end AI agent pipeline (ingestion → retrieval → generation)

---

## 🧠 System Architecture

1. **Document Ingestion**  
   - Upload PDF files  
   - Extract raw text  

2. **Preprocessing**  
   - Split text into manageable chunks  

3. **Embedding & Vector Store**  
   - Generate embeddings locally using SentenceTransformers  
   - Store embeddings in FAISS for similarity search  

4. **Retrieval-Augmented Generation (RAG)**  
   - Retrieve top relevant chunks  
   - Provide retrieved context to Gemini API  
   - Generate final answer grounded in document content  

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Platform:** Google Colab  
- **LLM:** Google Gemini (gemini-2.5-flash)  
- **Embeddings:** SentenceTransformers (local)  
- **Vector Database:** FAISS  
- **PDF Parsing:** PyMuPDF / pdfplumber  

---

## ⚙️ Installation & Setup (Google Colab)

1. Open Google Colab  
2. Upload the project notebook (`.ipynb`)  
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
4. Set your Gemini API key
5. Run the notebook cells step by step:

Upload PDFs

Build vector store

Ask questions
