📚 Multi-Doc RAG Chatbot

**Instant Intelligence from Multiple Documents**

OmniDoc AI is a high-performance, RAG-powered (Retrieval-Augmented Generation) chatbot designed to transform static document repositories into interactive knowledge bases. It allows users to query multiple PDF files simultaneously with sub-second inference speeds and human-like accuracy.

---

## 🚀 Project Overview

OmniDoc AI bridges the gap between massive unstructured PDF data and actionable insights. By combining the speed of the Groq LPU with the orchestration of LangChain, it provides a seamless chat experience where responses are strictly grounded in the provided documents, eliminating AI hallucinations.

---

## ⚠️ Problem Statement

- Information Overload: Searching through multiple 50+ page PDFs manually is time-consuming and inefficient.
- AI Hallucinations: Standard LLMs often invent facts when they lack specific context from private documents.
- Knowledge Cutoff: Commercial AI models cannot answer questions based on documents published after their training date.
- Latency Issues: Traditional RAG pipelines often suffer from slow processing times, hindering real-time utility.

---

## 💡 Solution

A multi-document RAG platform that utilizes Llama 3.1 and Vector Embeddings to act as a digital librarian. The system ingests, chunks, and indexes PDFs into a persistent vector database, allowing for contextual, conversational, and hyper-fast document querying.

---

## 🛠️ Key Features

- Multi-PDF Ingestion: Batch process and query across an entire directory of documents at once.
- Sub-Second Inference: Powered by Groq, providing lightning-fast responses using Llama 3.1 70B.
- Persistent Vector Storage: Uses ChromaDB to store document embeddings, ensuring data isn't re-processed on every run.
- Conversational Memory: Maintains full chat context, allowing for follow-up questions like "Can you explain that further?"
- Context Grounding: Responses include source verification, ensuring the AI only answers based on the uploaded data.

---

## 👤 User Roles
### 👑 Admin / Data Analyst

- Upload and manage the PDF document repository in the data/ folder.
- Execute the vectorized_documents.py script to update the knowledge base.
- Configure system prompts and model parameters (Temperature, Chunk Size).

### 💬 End User / Researcher

- Interact with the documents via a clean, intuitive Streamlit chat interface.
- Ask complex questions spanning across multiple different papers or reports.
- View real-time chat history and contextual responses.

## ⚙️ Technology Stack

- Orchestration: LangChain
- LLM: Llama 3.1 70B (via Groq Cloud API)
- Vector Database: ChromaDB
- Embeddings: HuggingFace (Sentence-Transformers)
- Frontend: Streamlit
- Document Processing: Unstructured & PDF Directory Loaders
- Environment: Python 3.10+

## 🎯 Future Enhancements

- Source Citations: Automatically highlighting the exact page and paragraph used for each answer.
- OCR Integration: Support for scanned images and handwritten documents using Tesseract or AWS Textract.
- Hybrid Search: Combining Keyword (BM25) and Vector search for even higher retrieval accuracy.
- Cloud Deployment: Containerization via Docker for deployment on AWS/GCP.

## 🌟 Key Benefits

- Accuracy: Eliminates "guessing" by forcing the model to retrieve facts from the Vector DB.
- Speed: Drastically reduces research time by summarizing thousands of pages in seconds.
- Privacy: Can be configured to run within a private environment, keeping sensitive documents secure.
- Scalability: Optimized to handle an increasing number of documents without significant performance drops.

## 📄 License

Academic & demonstration use only © 2026

## 👤 Author
Kanak Dharamthok
