
# AskPDFBot – Chat with Any PDF Using Local LLMs

AskPDFBot is a Streamlit-based chatbot that allows you to upload any PDF document and ask questions about its content using powerful local LLMs via Ollama. It leverages LangChain, ChromaDB for vector storage, and sentence-transformers for semantic search.

## Features

- 📄 Upload any PDF document
- 🤖 Ask questions and get contextual answers
- ⚡ Powered by **Ollama** for local LLM inference (e.g., `mistral`, `llama3`)
- 🔍 Uses **LangChain**, **ChromaDB**, and **sentence-transformers**
- 🖥️ Runs locally, no external API keys needed

## Tech Stack

- [Streamlit](https://streamlit.io) – Web UI
- [LangChain](https://www.langchain.com) – LLM orchestration
- [Ollama](https://ollama.com) – Local LLM server
- [ChromaDB](https://www.trychroma.com) – Vector DB
- [PyMuPDF](https://pymupdf.readthedocs.io) – PDF parsing
- [sentence-transformers](https://www.sbert.net/) – Embeddings
- [cross-encoder](https://huggingface.co/cross-encoder) – Reranking answers

## Installation

Make sure you have Python 3.10 or later installed.

### 1. Clone the Repo

```bash
git clone https://github.com/ram-rk-cmd/AskPDF
cd askpdfbot
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Install and Run Ollama

Go to [https://ollama.com](https://ollama.com) and install the app for your OS.

Then, pull a model and run it:

```bash
ollama pull mistral
ollama run mistral
```

### 4. Run the App

```bash
streamlit run app.py
```

## Example Usage

1. Open the app in your browser.
2. Upload a PDF document.
3. Type your question.
4. Get smart answers based on the document!

## requirements.txt

```txt
streamlit==1.45.1
chromadb==0.4.24
langchain==0.1.17
langchain-community==0.0.36
ollama==0.1.7
PyMuPDF==1.23.24
sentence-transformers==2.6.1
cross-encoder==0.1.6
```

## Future Improvements

- Chat history
- Multiple PDF support
- Option to choose models (LLaMA, Mistral, Phi, etc.)
- Online deployment (with optional remote model inference)

## License

MIT License
