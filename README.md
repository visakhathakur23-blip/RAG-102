# RAG – Retrieval-Augmented Generation

## Overview

This repository contains two implementations of Retrieval-Augmented Generation (RAG): **Typesense RAG** and **Agentic RAG**.

Both implementations explore semantic search and document-based question answering using vector embeddings and language models.

- **Typesense RAG:** Uses Typesense for storing and searching document information through semantic retrieval.
- **Agentic RAG:** Uses LangGraph to manage an agent workflow, FAISS for vector-based retrieval, Hugging Face embeddings, and Anthropic Claude for answer generation.

## Implementations

### 1. Typesense RAG

A document search and retrieval system that uses Typesense as its search engine.

**Features:**
- Load and process book data.
- Split text into smaller chunks.
- Generate embeddings using Hugging Face.
- Store and search documents using Typesense.
- Perform semantic document retrieval.

**Tech Stack:**
- Python
- LangChain
- Typesense
- Hugging Face Embeddings
- Jupyter Notebook

### 2. Agentic RAG

An agent-based RAG system that uses LangGraph to manage the retrieval and answer-generation workflow.

**Features:**
- Accept user questions.
- Decide whether document retrieval is required.
- Retrieve relevant documents using FAISS.
- Generate context-aware answers.
- Manage workflow execution using LangGraph.

**Tech Stack:**
- Python
- LangChain
- LangGraph
- FAISS
- Hugging Face Embeddings
- Anthropic Claude
- Jupyter Notebook

## Project Structure

```text
RAG/
├── Agentic rag/
│   ├── .env
│   └── agentic_rag.ipynb
│
├── VRAG/
│   ├── books.jsonl
│   ├── typesense.ipynb
│   └── requirements.txt
│
├── README.md
└── .gitignore
```

*Adjust folder and notebook names to match your actual GitHub repository.*

## Setup and Installation

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd YOUR_PROJECT_FOLDER
```

### 2. Install dependencies

Install the required packages for the implementation you want to run.

```bash
pip install -r requirements.txt
```

### 3. Configure environment variables

Create a `.env` file in the relevant project folder.

For Typesense RAG:

```env
TYPESENSE_HOST=your_typesense_host
TYPESENSE_API_KEY=your_typesense_api_key
```

For Agentic RAG:

```env
ANTHROPIC_API_KEY=your_anthropic_api_key
```

Never commit `.env` files or publish API keys.

### 4. Run the notebooks

Open the relevant Jupyter Notebook in VS Code or Jupyter Notebook and execute the cells in order.

## Applications

- Semantic document search
- Book information retrieval
- Document-based question answering
- Context-aware AI responses
- Agentic AI workflow experimentation

## Future Improvements

- Support PDF and DOCX document uploads.
- Add source citations to generated answers.
- Improve retrieval accuracy.
- Build an interactive chat interface.
- Evaluate retrieval and response quality.

## Author

**Visakha Thakur**

## License

This project is intended for educational and development purposes.
