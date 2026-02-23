# 🏥 Medical Chatbot: End-to-End RAG Pipeline

This repository contains a **professional-grade Medical Chatbot** powered by **Retrieval-Augmented Generation (RAG)**.

The system utilizes advanced NLP techniques to provide **context-aware, accurate answers** from medical documentation.

---

## 🚀 Tech Stack

* **Orchestration:** LangChain
* **Language:** Python
* **Web Framework:** Flask
* **Vector Database:** Pinecone
* **Cloud Hosting:** AWS (Amazon Web Services)
* **LLM:** Meta Llama / OpenAI (Configurable)
* **Embeddings:** Hugging Face / OpenAI

---

## 🏗️ Architecture Overview

The system follows a complete **RAG (Retrieval-Augmented Generation)** pipeline:

### 1️⃣ Data Ingestion

* Load medical PDFs or text documents using **LangChain document loaders**.

### 2️⃣ Chunking

* Split large documents into manageable chunks using:

  ```
  RecursiveCharacterTextSplitter
  ```

### 3️⃣ Embedding

* Convert text chunks into high-dimensional vector representations using:

  * Hugging Face Embeddings
  * OpenAI Embeddings

### 4️⃣ Vector Storage

* Store and index embeddings in **Pinecone** for efficient similarity search.

### 5️⃣ Retrieval

* Retrieve relevant context based on user queries using similarity search.

### 6️⃣ Generation

* Generate accurate, context-aware answers using:

  * Meta Llama
  * OpenAI LLM
* Implemented through a RAG chain in LangChain.

---

## 📂 Project Structure

```
medical-chatbot/
│
├── data/                 # Medical PDFs / documents
├── embeddings/           # Embedding generation scripts
├── vectorstore/          # Pinecone integration
├── app.py                # Flask application
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/medical-chatbot.git
cd medical-chatbot
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Configure Environment Variables

Create a `.env` file in the root directory:

```env
OPENAI_API_KEY=your_openai_key
PINECONE_API_KEY=your_pinecone_key
PINECONE_ENV=your_pinecone_environment
AWS_ACCESS_KEY_ID=your_aws_key
AWS_SECRET_ACCESS_KEY=your_aws_secret
```

---

## ▶️ Run the Application

```bash
python app.py
```

The chatbot will be available at:

```
http://127.0.0.1:5000
```

---

## 🌍 Deployment

This project can be deployed on:

* AWS EC2
* AWS Elastic Beanstalk
* Docker + AWS ECS
* Render / Railway (optional)

---

## 🔒 Disclaimer

This chatbot is intended for **educational and research purposes only**.
It should not replace professional medical advice, diagnosis, or treatment.

---

## 📌 Features

✔ End-to-End RAG Architecture
✔ Context-Aware Medical Responses
✔ Scalable Vector Database (Pinecone)
✔ Configurable LLM Backend
✔ Production-Ready Deployment Setup

