# VRAG –  Retrieval-Augmented Generation

## Overview
VRAG is a document search and retrieval project that uses vector search to find relevant information from a collection of books. It combines LangChain, Typesense, and Hugging Face embeddings to support semantic search and retrieval-augmented generation (RAG).

## Features
- Load and process documents.
- Split text into smaller chunks for efficient retrieval.
- Generate text embeddings using Hugging Face.
- Store and search documents using Typesense.
- Integrate with LangChain for document processing and retrieval.
- Use Anthropic Claude for language-model-powered responses.

## Tech Stack
- **Python**
- **LangChain**
- **Typesense**
- **Hugging Face Embeddings**
- **Anthropic Claude**
- **Jupyter Notebook**

## Project Structure
```text
VRAG/
├── src/
│   └── vrag/
│       └── __init__.py
├── books.jsonl
├── typesense.ipynb
├── requirements.txt
├── pyproject.toml
├── .python-version
├── .gitignore
└── README.md
```

## Setup and Installation

### 1. Clone the repository
```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd VRAG
```

### 2. Create a virtual environment
```bash
python -m venv .venv
```

Activate it on Windows:
```bash
.venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure environment variables
Create a `.env` file in the project root:

```env
TYPESENSE_HOST=your_typesense_host
TYPESENSE_API_KEY=your_typesense_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
```

Add any additional API keys required by your implementation. Never commit your `.env` file or publish API keys.

### 5. Run the project
Open `typesense.ipynb` in Jupyter Notebook or VS Code and run the cells in order.

## How It Works
1. Load documents from the source data.
2. Split documents into manageable text chunks.
3. Convert the chunks into vector embeddings.
4. Store and retrieve relevant information using Typesense.
5. Pass retrieved context to the language model to generate responses.

## Use Cases
- Semantic book search
- Document retrieval
- Context-aware question answering
- Retrieval-Augmented Generation experiments

## Future Improvements
- Add a user-friendly search interface.
- Improve document chunking and retrieval quality.
- Add source citations to generated answers.
- Implement evaluation for retrieval accuracy and response quality.

## Author
**Visakha Thakur **

## License
This project is for educational and development purposes. 
