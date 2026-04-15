# RAG-Document-Search-Engine

**🚀 [Live Demo: Try the RAG Document Search Engine Here](https://rag-document-search-engine-demo.streamlit.app/)**


An advanced **Retrieval-Augmented Generation (RAG)** system designed to transform static documents into an interactive, searchable knowledge base. This project leverages Large Language Models (LLMs) and Vector Databases to provide precise, context-aware answers to user queries based on uploaded PDF content.

---

## 🚀 Key Features

* **Contextual Search:** Goes beyond keyword matching by understanding the semantic meaning of your queries.
* **Multi-Document Support:** Ingest and process multiple PDF files simultaneously.
* **Vectorized Knowledge:** Utilizes high-performance vector embeddings to index document chunks for lightning-fast retrieval.
* **Interactive UI:** A clean, intuitive interface (built with Streamlit) for uploading documents and chatting with your data.
* **Source Attribution:** Provides transparency by referencing the specific sections of the documents used to generate answers.

---

## 🛠️ Tech Stack

* **Language:** Python 3.9+
* **LLM Framework:** [LangChain](https://www.langchain.com/) (Or similar framework used in the repo)
* **Vector Database:** [ChromaDB](https://www.trychroma.com/) / [FAISS](https://github.com/facebookresearch/faiss)
* **Embeddings:** OpenAI / HuggingFace Transformers
* **Frontend:** [Streamlit](https://streamlit.io/)

---

## 🏗️ How It Works


1.  **Ingestion:** PDFs are uploaded and decomposed into smaller, manageable text chunks.
2.  **Embedding:** Each chunk is converted into a high-dimensional vector representing its semantic meaning.
3.  **Indexing:** Vectors are stored in a specialized Vector Database for efficient similarity searching.
4.  **Retrieval:** When a user asks a question, the system finds the most relevant "context" chunks from the database.
5.  **Generation:** The LLM receives the user query + the retrieved context to generate a factual, grounded response.

---

## 🚦 Getting Started

### Prerequisites

* Python installed on your machine.
* An API Key for your chosen LLM provider (e.g., OpenAI, Anthropic, or a local Ollama instance).

### Installation

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/alpha9934/RAG-Document-Search-Engine.git
    cd RAG-Document-Search-Engine
    ```

2.  **Set Up a Virtual Environment**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Environment Variables**
    Create a `.env` file in the root directory and add your API credentials:
    ```env
    OPENAI_API_KEY=your_api_key_here
    ```

---

## 🖥️ Usage

Run the application using Streamlit:

```bash
streamlit run app.py
```

1.  Open your browser to the URL provided in the terminal (usually `http://localhost:8501`).
2.  Upload your PDF documents via the sidebar.
3.  Wait for the indexing process to complete.
4.  Start asking questions about your documents in the chat interface!

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

**Developed with ❤️ by [alpha9934](https://github.com/alpha9934)**
