# Conversation RAG with PDF Upload and Chat History

## Overview

This project implements a Retrieval-Augmented Generation (RAG) system using Langchain and Streamlit. It allows users to upload PDF documents, interact with a Q&A system, and maintain chat history for context-aware responses.

## Features

- **PDF Upload:** Upload and process PDF files.
- **Chat History:** Maintain and utilize chat history for context-aware responses.
- **Interactive Q&A:** Ask questions based on uploaded documents and get concise answers.
- **Secure API Integration:** Uses Groq and HuggingFace for language model capabilities.

## Setup Instructions

### Prerequisites

- Python 3.7 or higher
- Pip (Python package installer)

### Installation

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Required Libraries:**
   Use pip to install the necessary Python libraries:
   ```bash
   pip install streamlit langchain langchain-community langchain-groq langchain-huggingface langchain-text-splitters dotenv
   ```

3. **Set Up Environment Variables:**
   Create a `.env` file in the root of your project directory with the following content:
   ```plaintext
   HF_TOKEN=<your_huggingface_token>
   ```
   Replace `<your_huggingface_token>` with your HuggingFace token.

## Running the Application

1. **Save the Python Code:**
   Save the provided Python code into a file, e.g., `app.py`.

2. **Run Streamlit Application:**
   Start the Streamlit application with the following command:
   ```bash
   streamlit run app.py
   ```

3. **Access the Application:**
   Open a web browser and go to `http://localhost:8501` to interact with the application.

## Usage

1. **Upload PDF:**
   Use the file uploader to select and upload your PDF documents.

2. **Enter API Key:**
   Provide your Groq API key for language model access.

3. **Ask Questions:**
   Enter your questions into the provided input field to receive contextually relevant answers based on the uploaded PDF and chat history.

## Code Overview

- **Initialization:**
  Loads environment variables and initializes embeddings and language models.

- **PDF Handling:**
  Manages the upload and processing of PDF files.
  Splits documents into manageable chunks for better r
  etrieval performance.

- **Retrieval and Q&A:**
  Uses FAISS for document retrieval.
  Implements a history-aware retriever for context-aware responses.
  Provides concise answers based on the retrieved context.

## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your proposed changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the Langchain and Streamlit communities for their excellent libraries.
- Groq and HuggingFace for providing the language model capabilities.
