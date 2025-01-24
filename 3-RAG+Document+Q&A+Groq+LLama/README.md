# RAG+Document+Q&A+Groq+LLama

This project implements a **Retrieval-Augmented Generation (RAG)** system with **Groq** and **Llama3** for document-based question answering (Q&A). It allows users to interact with research papers and get contextually accurate answers using LangChain, Streamlit, and multiple embeddings.

---

## Project Structure

1. **app.py:**  
   The main Streamlit web application that allows users to interact with the system, input queries, and retrieve answers from the document database.

2. **requirements.txt:**  
   A file containing all the necessary dependencies for the project.

3. **research_papers/**  
   A folder that contains the research papers (PDFs) that will be loaded for document-based querying.

---

## Features

- **Document Embedding:**  
   Embeds documents (research papers) into a vector database using the HuggingFace embeddings.
  
- **Groq Integration:**  
   Uses Groq’s Llama3 model for answering questions based on the document context.
  
- **Real-Time Q&A:**  
   Provides real-time answers to user queries by fetching contextually relevant information from embedded documents.
  
- **Document Similarity Search:**  
   Allows for document similarity search and displays the context used to generate the answer.

---

## Installation and Setup

### Prerequisites

1. **Python 3.7 or higher**  
   Ensure Python 3.7 or higher is installed.

2. **Anaconda or Miniconda Installed:**  
   Install Miniconda or Anaconda if you don’t already have it. You can download it from [here](https://www.anaconda.com/products/individual).

### Setting Up the Environment

1. **Clone the Repository:**
   ```bash
   git clone <repository_url>
   cd <repository_folder>
   
2. Create a Conda Environment:
    bash
    conda create -n rag-gen-ai-search python=3.8 -y
   
4. Activate the Environment:
    bash
    conda activate rag-gen-ai-search
   
4. Install Dependencies:
   Install the required libraries using requirements.txt:

    bash
    pip install -r requirements.txt
   
5. Set Up Environment Variables:
   Create a .env file in the project root with the following content:
    bash
    OPENAI_API_KEY=your_openai_api_key
    GROQ_API_KEY=your_groq_api_key
    HF_TOKEN=your_huggingface_token
   
How to Run
1. Run the Streamlit App:
   Start the app by executing:
    bash
    streamlit run app.py
   
2. Interact with the App:

   .  Enter your query in the chat input (e.g., "What is machine learning?").
   . Click on "Document Embedding" to load and process the research papers.
   . View responses generated in real time based on the documents.
   
3.Document Similarity Search:
  You can expand the search results to view the context from the documents that helped answer your query.

Code Overview
Initialization:
The app loads the API keys, initializes embeddings, and loads the research papers.

Document Processing:
Research papers are embedded into a vector database for efficient retrieval and querying.

Q&A Generation:
User queries are processed with a prompt template to ensure accurate answers based on the document context.

Document Retrieval:
FAISS is used for efficient document retrieval, and the context is passed to the Llama3 model to generate answers.

