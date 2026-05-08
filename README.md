# 🤖📄 ChatPDF – Interactive RAG-Based PDF Assistant

Welcome to **ChatPDF**, where your documents talk back to you.

Instead of scrolling through long PDFs, you can simply *ask questions* and get precise answers powered by AI.

---

## 🎯 What Can You Do With This?

👉 Upload one or more PDF files
👉 Ask questions in natural language
👉 Get accurate, context-based answers instantly

💡 Think of it like **ChatGPT for your own documents**.

---

## 🧠 How It Works (Simple View)

🪄 Step 1: Upload PDFs
📖 Step 2: Text is extracted
✂️ Step 3: Text is split into chunks
🔢 Step 4: Converted into embeddings
📦 Step 5: Stored in FAISS vector DB
🔍 Step 6: Relevant chunks retrieved
🤖 Step 7: Gemini generates the answer

👉 This approach is called **RAG (Retrieval-Augmented Generation)**

---

## 🖥️ Demo Flow

1. Open the app
2. Upload PDFs from sidebar
3. Click **Submit & Process**
4. Ask a question
5. Get your answer 🎉

---

## 🛠️ Tech Stack

| Component       | Technology Used      |
| --------------- | -------------------- |
| Frontend        | Streamlit            |
| LLM             | Google Gemini        |
| Embeddings      | Google Generative AI |
| Vector Database | FAISS                |
| Framework       | LangChain            |
| PDF Reader      | PyPDF2               |

---

## ⚙️ Setup Guide (Step-by-Step)

### 📥 1. Clone Repository

```
git clone https://github.com/your-username/chatpdf-rag.git
cd chatpdf-rag
```

### 📦 2. Install Dependencies

```
pip install -r requirements.txt
```

### 🔑 3. Add API Key

Create a `.env` file:

```
GOOGLE_API_KEY=your_api_key_here
```

⚠️ Never upload this file to GitHub.

### ▶️ 4. Run the App

```
streamlit run chatpdf1.py
```

---

## ✨ Key Features

✅ Multi-PDF Support
✅ Fast Semantic Search
✅ Context-Aware Answers
✅ Easy-to-use Interface
✅ Reduces AI hallucination

---

## 🧪 Try Asking Questions Like:

💬 "Summarize this document"
💬 "What are the key points?"
💬 "Explain the conclusion"
💬 "Find details about XYZ topic"

---

## 📂 Project Structure

```
chatpdf-rag/
│── chatpdf1.py
│── requirements.txt
│── .env (not shared)
│── faiss_index/
│── README.md
```

---

## ⚠️ Important Notes

❌ Do NOT expose your API key
❌ Do NOT upload `.env` file

✔ Use environment variables properly:

```
os.getenv("GOOGLE_API_KEY")
```

---

## 🚀 Future Improvements

🔹 Chat history (memory)
🔹 Better UI design
🔹 PDF highlighting
🔹 Deployment (Hugging Face / Cloud)
🔹 Support more file formats

---

## 👨‍💻 Author

Harish Maheshkumar 

---

## ⭐ Final Thought

This project demonstrates how to combine **LLMs + Vector Search** to build real-world AI applications.

👉 Not just a chatbot — a **smart document assistant**.
