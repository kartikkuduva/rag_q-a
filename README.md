

📘 Q&A Retrieval-Augmented Generation (RAG)

This project implements a Q&A system using Retrieval-Augmented Generation (RAG).
It allows users to upload documents (e.g., invoices in PDF format), process them into chunks, store embeddings in a vector database, and query them using Groq LLM with LangChain.

🚀 Features

1. Load PDF documents using LangChain’s PyPDFLoader

2. Extract and chunk text for efficient retrieval

3. Generate embeddings using Hugging Face models

4. Store embeddings in a vector database for semantic search

5. Query documents in natural language using Groq API LLM

6. Get contextual answers based on document content

🛠️ Tech Stack

Python 3.11+

LangChain

Groq API

Hugging Face Transformers

dotenv (for managing API keys)

PyPDFLoader (for loading PDFs)

📂 Project Structure
Q&A_rag.ipynb     # Main Jupyter Notebook with the pipeline
Data/             # Folder for storing input PDF documents

⚙️ Setup Instructions

Clone the repository

git clone <your-repo-url>
cd <repo-folder>


Create and activate a virtual environment

python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows


Install dependencies

pip install -r requirements.txt


Set environment variables
Create a .env file in the root directory:

GROQ_API_KEY=your_groq_api_key
huggingface_api=your_huggingface_api_token

▶️ Running the Project

1. Place your PDF file (e.g., invoices) in the Data/ folder.

2. Open the notebook:

   jupyter notebook Q&A_rag.ipynb

3. Run the cells step by step:

* Load and preprocess documents

* Create embeddings

* Store/retrieve chunks

* Query documents with natural language

💡 Example Queries

"What is the invoice number?"

"Who is the customer?"

"What is the total amount billed?"

📌 Future Improvements

Add support for multiple document formats (DOCX, TXT).

Deploy as a Streamlit/Gradio web app for interactive querying.

Integrate advanced vector databases (e.g., Pinecone, Weaviate, FAISS).
