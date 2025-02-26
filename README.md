# Document-based-Chatbot-using-RAG
A Q&amp;A chatbot using Retrieval-Augmented Generation (RAG) with ChromaDB and LLaMA 3.1 (via Groq). It extracts text from a PDF, generates embeddings using Hugging Face, stores them in ChromaDB, retrieves relevant chunks based on similarity scores, and summarizes the retrieved content using an LLM before returning an answer

# RAG-Based Q&A Chatbot with ChromaDB & LLaMA 3.1 (Groq)

## 📌 Project Overview
This project is a **Q&A chatbot** that utilizes **Retrieval-Augmented Generation (RAG)** to answer questions based on a provided **PDF document**. It follows these steps:
1. **Extract text from a PDF** using `PyPDFLoader`.
2. **Split text into chunks** for efficient retrieval.
3. **Generate embeddings** using `HuggingFaceEmbeddings`.
4. **Store embeddings** in `ChromaDB`.
5. **Retrieve relevant chunks** based on similarity scores.
6. **Summarize retrieved information** using `LLaMA 3.1 (via Groq)`.
7. **Return the summarized answer** to the user.

## 🛠️ Tech Stack
- **Python**
- **LangChain**
- **ChromaDB**
- **Groq API (LLaMA 3.1)**
- **Hugging Face Embeddings**
- **PyPDFLoader**

## 🚀 Installation

### 1️⃣ Clone the repository:
```bash
git clone https://github.com/kedarhardikar/Document-based-Chatbot-using-RAG.git

### 2️⃣ Create a virtual environment:
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate     # On Windows

### 3️⃣ Install dependencies:
pip install -r requirements.txt

### 4️⃣ Set up environment variables:
Create a .env file in the root directory and add:
GROQ_API_KEY=your_api_key_here
Get your Groq API key from https://console.groq.com/keys

### 5️⃣ Run the chatbot:
python main.py

### Project Structure
📂 rag-qna-chatbot
│── 📄 final.py                # Main script for the chatbot
│── 📄 requirements.txt       # Required dependencies
│── 📄 README.md              # Project documentation
│── 📄 .env                   # API key storage (not included in Git)
│── 📂 chroma_db              # ChromaDB storage (not included in Git)
│── 📄 doc.pdf                # Input PDF document

### Example usage
Ask a question (or type 'exit' to quit): What is the summary of the document?
Summary:
[Generated answer based on PDF]





