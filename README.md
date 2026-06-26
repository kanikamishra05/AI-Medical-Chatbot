# AI Medical Chatbot (RAG-based)

An AI-powered Medical Chatbot built using Retrieval-Augmented Generation (RAG). The chatbot retrieves relevant information from medical PDF documents using Pinecone vector search and generates context-aware responses with OpenAI GPT-4o.

## Features

- Retrieval-Augmented Generation (RAG)
- Medical PDF document processing
- Semantic search using Pinecone
- Hugging Face sentence embeddings
- GPT-4o powered responses
- Flask web interface

## Tech Stack

- Python
- Flask
- LangChain
- OpenAI GPT-4o
- Hugging Face Embeddings
- Pinecone Vector Database

## Project Structure

```
data/          # Medical PDF files
src/           # Helper functions and prompts
templates/     # HTML templates
static/        # CSS and static assets
app.py         # Flask application
store_index.py # Creates embeddings and stores them in Pinecone
```

## Installation

Clone the repository:

```bash
git clone https://github.com/kanikamishra05/AI-Medical-Chatbot.git
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it:

Windows

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create a `.env` file:

```env
PINECONE_API_KEY=YOUR_PINECONE_API_KEY
OPENAI_API_KEY=YOUR_OPENAI_API_KEY
```

Create the vector database:

```bash
python store_index.py
```

Run the application:

```bash
python app.py
```

Open:

```
http://localhost:8080
```

## Future Improvements

- PDF upload through UI
- Chat history
- Source citations
- Docker deployment
- Cloud deployment