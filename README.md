# RAG Datasheet QA System

This project is a Retrieval-Augmented Generation (RAG) based question answering system for technical datasheets. It allows users to upload a datasheet, indexes the document using vector embeddings, and answers questions by retrieving the most relevant sections before generating a response using the Groq LLM.

## Features

- Upload and process PDF datasheets
- Create vector embeddings for efficient retrieval
- Retrieve relevant document chunks based on user queries
- Generate context-aware answers using Groq
- Interactive notebook implementation

## Requirements

- Python 3.10 or later
- Jupyter Notebook
- A Groq API key

Install the required packages before running the notebook:

```bash
pip install -r requirements.txt
```

If a `requirements.txt` file is not included, install the libraries used in the notebook manually.

## Getting a Groq API Key

1. Create an account at https://console.groq.com/.
2. Generate a new API key from the dashboard.
3. Add the key where the notebook expects it, or set it as an environment variable.

Example:

```python
import os
os.environ["GROQ_API_KEY"] = "your_api_key_here"
```

Alternatively, you can store it in a `.env` file if your notebook uses `python-dotenv`.

## Running the Project

1. Clone this repository.
2. Install the required Python packages.
3. Configure your Groq API key.
4. Open the Jupyter notebook.
5. Run the cells from top to bottom.
6. Upload a supported datasheet when prompted.
7. Ask questions about the uploaded document.

## Notes

- Make sure your Groq API key is valid before running the notebook.
- Large documents may take a little longer to process during the indexing step.
- Do not commit your API key or `.env` file to GitHub.

## Future Improvements

- Support multiple document uploads
- Add a web interface using Streamlit or Flask
- Store vector embeddings for faster reuse
- Support additional LLM providers
