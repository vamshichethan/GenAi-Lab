# News Research Tool

This is a Streamlit-based RAG app I built to research news articles. The app accepts article URLs, creates embeddings with LangChain, stores them in FAISS, and answers questions with source references.

![News Research Tool](rockybot.jpg)

## Features

- Load article URLs from the sidebar.
- Extract and split article content with LangChain.
- Create OpenAI embeddings and store them with FAISS.
- Ask questions and receive answers with source URLs.

## Setup

```bash
pip install -r requirements.txt
cp .env.example .env
```

Add your OpenAI API key in `.env`.

## Run

```bash
streamlit run main.py
```

## Files

- `main.py` - Streamlit app.
- `requirements.txt` - Python dependencies.
- `.env.example` - Sample environment file.
- `notebooks/` - experiments for loaders, splitters, FAISS, and retrieval.
