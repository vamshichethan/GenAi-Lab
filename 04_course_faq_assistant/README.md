# Course FAQ Assistant

This is a question-answering assistant built over a CSV FAQ knowledge base. I used LangChain, Google PaLM, Hugging Face embeddings, FAISS, and Streamlit to create a simple support-style interface.

![Course FAQ Assistant](codebasics_q_and_a.png)

## Project Highlights

- Loads FAQ data from CSV.
- Builds a local FAISS knowledge base.
- Retrieves relevant FAQ context for each question.
- Answers only from the provided knowledge base.

## Setup

```bash
pip install -r requirements.txt
cp .env.example .env
```

Add your Google API key in `.env`.

## Run

```bash
streamlit run main.py
```

Click the create knowledge base button on the first run, then type a question and press Enter.

## Sample Questions

- Do you provide internships and EMI payments?
- Do you have a JavaScript course?
- Should I learn Power BI or Tableau?
- Can I use Power BI on a Mac?

## Files

- `main.py` - Streamlit UI.
- `langchain_helper.py` - LangChain retrieval chain logic.
- `codebasics_faqs.csv` - FAQ knowledge base.
- `.env.example` - Sample environment file.
