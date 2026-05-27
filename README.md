# GenAI Lab

A hands-on collection of Generative AI and LangChain projects that I built while learning how LLM apps work end to end. This repo brings together my experiments with prompt chains, Streamlit apps, vector search, retrieval augmented generation, and natural-language database querying.

I started these projects by following along with YouTube learning material, then organized the code as my own lab so I can keep improving it, reuse patterns, and show the complete learning path in one place.

## What I Built

| Folder | Project | What it does |
| --- | --- | --- |
| `01_langchain_basics` | LangChain basics | Notebook experiments for chains, prompts, LLM calls, and core LangChain concepts. |
| `02_restaurant_name_generator` | Restaurant Name Generator | Streamlit app that uses chained prompts to generate a restaurant name and menu ideas from a cuisine. |
| `03_news_research_tool` | News Research Tool | RAG app that loads article URLs, builds FAISS embeddings, and answers questions with source references. |
| `04_course_faq_assistant` | Course FAQ Assistant | Q&A assistant over a CSV knowledge base using embeddings, FAISS, LangChain, and Google PaLM. |
| `05_sql_tshirt_store_assistant` | SQL T-Shirt Store Assistant | Natural-language database assistant that turns business questions into SQL over a MySQL inventory database. |

## Tech Stack

- Python
- Streamlit
- LangChain
- OpenAI API
- Google PaLM API
- FAISS
- ChromaDB
- Hugging Face embeddings
- MySQL
- Jupyter Notebook

## Project Structure

```text
GenAi-Lab/
├── 01_langchain_basics/
├── 02_restaurant_name_generator/
├── 03_news_research_tool/
├── 04_course_faq_assistant/
├── 05_sql_tshirt_store_assistant/
└── README.md
```

Each project folder has its own `README.md`, `requirements.txt` where needed, and app/notebook files.

## Setup

Clone the repository:

```bash
git clone https://github.com/vamshichethan/GenAi-Lab.git
cd GenAi-Lab
```

Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

Install dependencies for the project you want to run:

```bash
cd 03_news_research_tool
pip install -r requirements.txt
```

Create a `.env` file from the sample file in that project folder and add your API key:

```bash
cp .env.example .env
```

## Running Streamlit Apps

From inside any Streamlit project folder:

```bash
streamlit run main.py
```

## Notes

- API keys and local `.env` files are intentionally ignored.
- Generated vector stores such as FAISS/Chroma indexes are ignored because they can be recreated from the app.
- The database project needs a local MySQL database created from the SQL file in `05_sql_tshirt_store_assistant/database/`.

## Learning Outcome

This repo helped me understand how GenAI apps are assembled beyond a single prompt: loading data, splitting documents, creating embeddings, storing vectors, retrieving context, building chains, and connecting LLMs to real interfaces like Streamlit and SQL databases.
