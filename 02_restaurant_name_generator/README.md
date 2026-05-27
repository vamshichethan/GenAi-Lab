# Restaurant Name Generator

This is a small Streamlit app that generates a restaurant name and menu items based on the cuisine selected by the user. I used it to practice prompt templates and sequential chains in LangChain.

## Features

- Select a cuisine from the sidebar.
- Generate a restaurant name with an LLM prompt.
- Pass the generated name into a second prompt to create menu items.
- Display the result in a simple Streamlit UI.

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

- `main.py` - Streamlit UI.
- `langchain_helper.py` - LangChain prompt and chain logic.
- `.env.example` - Sample environment file.
