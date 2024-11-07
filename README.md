# Document Question-Answering with RAG and Google Gemini API

This project demonstrates how to use **Retrieval-Augmented Generation (RAG)** and Google's **Gemini API** with **LangChain** to build a question-answering system that interacts with PDF documents. By extracting text from documents and employing a retrieval mechanism, this tool enables users to ask natural language questions and receive accurate, context-based answers.

## Features
- **Question-Answering with Documents**: Ask questions about a document, and receive detailed, contextually relevant answers.
- **Text Extraction from PDFs**: Converts PDF documents into readable text format for easy querying.
- **RAG with Vector Database**: Uses **ChromaDB** to retrieve relevant document sections, improving the relevance of answers.
- **Language Model Integration**: Integrates **Google’s Gemini API** via LangChain for advanced language generation and understanding.

## Tech Stack
- **Python**: Core programming language for building the project.
- **Google Gemini API**: Provides language model capabilities to generate responses.
- **LangChain**: Manages the flow and interaction between the user, retrieval system, and Gemini API.
- **ChromaDB**: A vector database used to store and retrieve document segments efficiently.
- **pypdf**: Extracts text from PDF files to prepare them for question-answering.
- **Jupyter Notebook**: Used to build and run the project interactively.

## Installation

1. **Clone this repository**:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   
2. **Install required packages**:
   ```bash
   pip install -q --upgrade google-generativeai langchain-google-genai chromadb pypdf

3. Set up your Google Gemini API key as an environment variable:
   ```bash
   export GOOGLE_API_KEY=your_google_api_key

##  Usage

1. **Load and Process a PDF**:
    Run the notebook or script to load a PDF document and extract its text content.
    
2. **Ask Questions**:
    Use the question-answering interface to ask questions about the document. The system will retrieve relevant segments and generate a detailed answer.
    Example Questions:
    - "What is the main theme of this document?"
    - "Explain section 2 in detail."

## Code Structure
- **PDF Text Extraction**: Extracts and cleans text from the uploaded PDF.
- **RAG Pipeline**: Combines retrieval and language generation to provide contextually accurate answers.
- **Gemini Integration**: Uses LangChain to interact with Google’s Gemini API for language model responses.
