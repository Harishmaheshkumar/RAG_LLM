# 📄 RAG-Based PDF Interaction Chatbot

An end-to-end **Retrieval-Augmented Generation (RAG)** application that allows users to interact with PDF documents using natural language. The system retrieves relevant document context using **FAISS vector search** and generates accurate, grounded answers using **Google Gemini API**, significantly reducing hallucinations compared to standalone LLMs.

---

## 🚀 Features

* 📑 Upload and query PDF documents
* 🔍 Semantic search using embeddings + FAISS
* 🤖 Context-aware responses powered by Google Gemini
* 🧠 Reduces hallucinations via retrieval grounding
* 🔄 Supports multi-question workflows
* ⚡ Fast local vector search

---

## 🏗️ System Architecture

1. **PDF Ingestion** – Upload and extract text from PDF files
2. **Text Chunking** – Split large text into smaller, meaningful chunks
3. **Embedding Generation** – Convert chunks into dense vector embeddings
4. **Vector Store (FAISS)** – Store and index embeddings for similarity search
5. **Query Processing** – Embed user query and retrieve top-k relevant chunks
6. **Answer Generation** – Pass retrieved context + query to Gemini LLM

> "Retrieve first, then generate" – ensures factual, document-grounded responses.

---

## 🧰 Tech Stack

* **Language:** Python
* **LLM:** Google Gemini API
* **Vector Database:** FAISS
* **Embeddings:** Gemini / compatible embedding model
* **Libraries:** LangChain, PyPDF, NumPy
* **Environment:** Python 3.9+

---

## 📁 Project Structure

```
RAG_LLM/
│── chatpdf1.py        # Main application logic
│── requirements.txt  # Project dependencies
│── .env               # API keys and environment variables
│── README.md          # Project documentation
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Harishmaheshkumar/RAG_LLM.git
cd RAG_LLM
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Configure Environment Variables

Create a `.env` file:

```
GOOGLE_API_KEY=your_gemini_api_key
```

---

## ▶️ How to Run

```bash
python chatpdf1.py
```

* Upload a PDF
* Ask questions in natural language
* Get accurate, context-aware answers

---

## 🧠 Why RAG?

* ❌ LLM-only systems hallucinate
* ❌ Cannot access private documents
* ❌ Token limitations

✅ RAG solves these by grounding responses in retrieved document context.

---

## 📊 Evaluation

* Manual qualitative testing with real user queries
* Compared LLM-only vs RAG-based answers
* Observed improved factual accuracy and reduced hallucinations

---

## ⚠️ Limitations

* Performance depends on PDF text quality
* Scanned PDFs require OCR
* Large PDFs increase indexing time
* Stateless conversations (no long-term memory)

---

## 🔮 Future Enhancements

* Add OCR support for scanned PDFs
* Implement hybrid search (BM25 + embeddings)
* Add persistent vector databases (Pinecone / Weaviate)
* Enable multi-document querying
* Dockerize for deployment

---

## 👨‍💻 Author

**Harish M**
AI & ML Enthusiast | Data Science | Generative AI

* 🔗 GitHub: [https://github.com/Harishmaheshkumar](https://github.com/Harishmaheshkumar)
* 🔗 LinkedIn: [https://www.linkedin.com/in/harish-maheshkumar](https://www.linkedin.com/in/harish-maheshkumar)

---

⭐ If you like this project, give it a star!
