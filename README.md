# Sales Call Analysis using LangChain and ChromaDB

## Overview
This project processes sales call conversation transcripts and evaluates the salesperson's performance using an AI-driven retrieval system. The system leverages LangChain, ChromaDB, and Hugging Face embeddings to analyze the conversation and answer predefined queries based on the call's context.

## Features
- **Document Processing**: Supports PDF and TXT file formats for processing call transcripts.
- **Text Chunking**: Splits documents into smaller chunks for efficient embedding.
- **Vector Store with ChromaDB**: Stores and retrieves relevant chunks using sentence embeddings.
- **Query-Based Evaluation**: Uses LangChain and ChatGroq to provide AI-generated insights for sales performance evaluation.

## Technologies Used
- Python
- LangChain
- Hugging Face Embeddings (`sentence-transformers/all-MiniLM-L6-v2`)
- ChromaDB
- ChatGroq (`mixtral-8x7b-32768`)
- PyPDFLoader (for PDF processing)
- RecursiveCharacterTextSplitter (for chunking documents)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
