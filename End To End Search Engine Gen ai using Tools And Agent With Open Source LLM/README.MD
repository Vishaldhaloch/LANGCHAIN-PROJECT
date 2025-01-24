End-to-End Generative AI Search Engine using Gen ai Tools and Agents With Open Source LLM
This project is an End-to-End Generative AI Search Engine that uses LangChain, Streamlit, and an open-source LLM to answer user queries. The system integrates tools like Arxiv, Wikipedia, and DuckDuckGo search to provide contextual, real-time information, all wrapped in an interactive web app.

Project Structure
toolagent.ipynb
Contains the configuration for LangChain tools and custom retrievers. This file handles the initialization of the tools and LLM used for building the agent.

app.py
A Streamlit-based web application that interacts with the agent, processes user queries, and displays results interactively. The app uses LangChain's StreamlitCallbackHandler to show real-time interactions.

requirements.txt
A file containing all the necessary dependencies for the project.

Features
Wikipedia Search: Fetches short, concise summaries from Wikipedia.
Arxiv Search: Retrieves research paper summaries using Arxiv APIs.
DuckDuckGo Search: Provides real-time web search capabilities.
Interactive Chat Interface: Powered by Streamlit, allowing easy and intuitive interaction with the system.
Open Source LLM Integration: Uses Groq-based LLM (Llama3) for natural language processing and reasoning.

Installation and Setup

Prerequisites
Anaconda or Miniconda Installed:
Install Miniconda or Anaconda if you don’t already have it. You can download it from here.

Setting Up the Environment
Clone the Repository:

bash
git clone <repository_url>
cd <repository_folder>

Create a Conda Environment:

bash
conda create -n gen-ai-search python=3.8 -y

Activate the Environment:

bash
conda activate gen-ai-search

Install Dependencies: Install the required libraries using requirements.txt:

bash

pip install -r requirements.txt

Set Up Environment Variables: Create a .env file in the project root with the following content:

bash

GROQ_API_KEY=your_groq_api_key

How to Run
Set Up the Tools (Optional): Open toolagent.ipynb in a Jupyter Notebook and run all cells to ensure the tools and agents are set up correctly.

Run the Streamlit App: 
Start the app by executing:

bash

streamlit run app.py
Interact with the App:

Enter your Groq API Key in the sidebar.
Type your query in the chat input (e.g., "What is machine learning?").
View responses generated in real time.

How It Works
Tool Configuration:
The toolagent.ipynb file configures Wikipedia, Arxiv, and DuckDuckGo tools, along with the LLM, and prepares them for use.

Streamlit App:
The app.py file initializes the chat interface. Users input queries, which are processed by the agent using the tools and the Groq-powered LLM.

Real-Time Feedback:
Responses from the agent are displayed live, with intermediate steps visible for transparency.

 











