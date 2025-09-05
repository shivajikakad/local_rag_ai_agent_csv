# Local RAG AI Agent for Pizza Restaurant Reviews

This project is a Python-based local AI agent that answers questions about a pizza restaurant using customer reviews stored in CSV format. It leverages LangChain for prompt and model chaining, Ollama for local LLM inference, and Chroma for vector-based retrieval.

## Features
- Interactive Q&A about a pizza restaurant
- Uses real customer reviews for context
- Local language model inference (Ollama)
- Fast vector search with Chroma

## How It Works
1. User asks a question about the restaurant.
2. The agent retrieves relevant reviews using Chroma vector search.
3. The reviews and question are formatted into a prompt.
4. The prompt is sent to a local LLM (Ollama) for an answer.

## Requirements
- Python 3.10+
- [Ollama](https://ollama.com/) installed and running
- Required Python packages (see `requirements.txt`):
  - langchain
  - langchain-ollama
  - langchain-chroma
  - pandas

## Setup
1. Clone this repository.
2. Create and activate a Python virtual environment:
   ```powershell
   python -m venv venv
   .\venv\Scripts\Activate.ps1
   ```
3. Install dependencies:
   ```powershell
   pip install -r requirements.txt
   ```
4. Ensure Ollama is running locally.
5. Run the program:
   ```powershell
   python main.py
   ```

## Usage
- Enter your question when prompted.
- Type `q` to quit.

## File Structure
- `main.py` — Main program logic
- `vector.py` — Vector search and retrieval
- `realistic_restaurant_reviews.csv` — Source reviews
- `requirements.txt` — Python dependencies
- `chrome_langchain_db/` — Chroma vector database

## License
This project is for educational and demonstration purposes.
