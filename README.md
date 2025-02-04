#Sales Call Analysis using LangChain and ChromaDB

Overview

This project processes sales call conversation transcripts and evaluates the salesperson's performance using an AI-driven retrieval system. The system leverages LangChain, ChromaDB, and Hugging Face embeddings to analyze the conversation and answer predefined queries based on the call's context.

Features

Document Processing: Supports PDF and TXT file formats for processing call transcripts.

Text Chunking: Splits documents into smaller chunks for efficient embedding.

Vector Store with ChromaDB: Stores and retrieves relevant chunks using sentence embeddings.

Query-Based Evaluation: Uses LangChain and ChatGroq to provide AI-generated insights for sales performance evaluation.

Technologies Used

Python

LangChain

Hugging Face Embeddings (sentence-transformers/all-MiniLM-L6-v2)

ChromaDB

ChatGroq (mixtral-8x7b-32768)

PyPDFLoader (for PDF processing)

RecursiveCharacterTextSplitter (for chunking documents)

Installation

Clone the repository:

git clone https://github.com/yourusername/your-repo.git
cd your-repo

Install required dependencies:

pip install -r requirements.txt

Set up the environment variables (e.g., for groq_api_key).

Usage

Process a document

Place the call transcript (PDF/TXT) in the appropriate directory.

Update document_path in the script with the actual file path.

Run the script

python script.py

Provide queries

Add queries in salesqueries.txt (one per line) to evaluate the sales conversation.

View the responses

The script will analyze the conversation and print the evaluation results.

File Structure

/
│── script.py                  # Main script for processing documents and running queries
│── requirements.txt           # List of dependencies
│── salesqueries.txt           # File containing evaluation queries
│── data/                      # Directory to store input transcripts
│── chroma_db/                 # Directory storing ChromaDB vector store

Future Enhancements

Add support for .docx files.

Improve response formatting and output storage.

Integrate a web-based interface for easier interaction.

License

This project is licensed under the MIT License.
