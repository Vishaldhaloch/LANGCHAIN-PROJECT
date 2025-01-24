# Conversational RAG With PDF Uploads and Chat History  

This project is a **Conversational Retrieval-Augmented Generation (RAG) application** built with Streamlit. It allows users to:  
- Upload PDF documents  
- Extract and process their content  
- Interact with the extracted data in a conversational way  

The application maintains a **chat history** for better context during interactions.  

---

## Features  

- **Upload PDFs:** Upload one or multiple PDF files to extract content.  
- **Text Embeddings:** Uses the `all-MiniLM-L6-v2` model to generate embeddings for document content.  
- **Chroma Vector Store:** Stores and retrieves document embeddings for fast, relevant responses.  
- **Context-Aware Q&A:** Reformulates questions based on chat history for better context.  
- **Streamlit UI:** Simple and interactive web interface for uploading files and chatting.  
- **Session Management:** Maintains chat history across sessions for continuity.  

---

## Overview  

The **Conversational RAG with PDF Uploads** combines cutting-edge natural language processing techniques to enable seamless interaction with document-based content.  

Key components include:  
- **PDF Parsing and Processing:** Extract text from uploaded PDFs.  
- **Document Embeddings:** Use pre-trained models to create semantic embeddings of the document content.  
- **Chroma Vector Store:** Efficiently store and retrieve document embeddings to provide contextually relevant answers.  
- **Conversational AI:** With `ChatGroq`, the system delivers coherent and concise responses while considering chat history for improved context understanding.  
- **Streamlit Frontend:** An intuitive user interface for managing files and interacting with the system.  

This tool is ideal for individuals or organizations looking to interact with large volumes of PDF-based information without manually reading through documents.  

---

## Setup  

### Prerequisites  

- Python 3.9 or above  
- An account with Groq and the Groq API key  
- Hugging Face API token  

### Installation  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/yourusername/conversational-rag-pdf.git  
   cd conversational-rag-pdf  
2. Create a virtual environment:
   
   python -m venv env  
   source env/bin/activate  # On Windows: `env\Scripts\activate`
4. Install dependencies:
   
   pip install -r requirements.txt
   
6. Create a .env file in the root directory and add your API tokens:
   HF_TOKEN=your_huggingface_api_key


Usage
1. Run the Streamlit app:
   streamlit run app.py
   
2. Open the web interface in your browser (default: http://localhost:8501).

3. Enter your Groq API key in the provided input field.

4. Upload PDF files and start interacting with their content through chat!



