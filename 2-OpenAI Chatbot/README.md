# Enhanced Q&A Chatbot with OpenAI

This project implements an **Enhanced Q&A Chatbot** using **OpenAI's GPT models**. It allows users to interact with a chatbot powered by OpenAI's API. The system provides context-based answers based on the user's queries and includes adjustable settings for response customization.

---

## Project Structure

1. **app.py**  
   The main Streamlit web application that allows users to interact with the chatbot, enter their questions, and customize the settings.

2. **requirements.txt**  
   A file containing all the necessary dependencies for the project.

---

## Features

- **Interactive Chat Interface:**  
   Powered by Streamlit, the chatbot allows users to ask questions and receive responses in real time.

- **OpenAI Integration:**  
   Uses OpenAI’s GPT-4 models for generating responses based on the user input.

- **Customizable Settings:**  
   Users can input their OpenAI API key, select the model, and adjust the response settings like temperature and maximum token length.

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
   
2.**Create a Conda Environment:**
    ```bash
    conda create -n openai-chatbot python=3.8 -y

3.**Activate the Environment:**
    ```bash
    conda activate openai-chatbot
  
4.**Install Dependencies:**
  Install the required libraries using requirements.txt:
    ```bash
    pip install -r requirements.txt
   
5.**Set Up Environment Variables:**
  Create a .env file in the project root with the following content:
    ```bash
    OPENAI_API_KEY=your_openai_api_key
    LANGCHAIN_API_KEY=your_langchain_api_key
   
**How to Run**
1.Run the Streamlit App:
Start the app by executing:
  ```bash
  streamlit run app.py
 
2.**Interact with the Chatbot:**

   1.Enter your OpenAI API Key in the sidebar.
   2.Select the OpenAI model (e.g., gpt-4, gpt-4-turbo).
   3.Adjust response parameters such as temperature and max tokens.
   4.Ask any question in the main interface, and the chatbot will provide an answer in real time.
  
**Code Overview**
  Initialization:
  The app initializes the API keys and sets up the LangChain API key for tracking.

**Prompt Template:**
  The prompt template is designed to ensure the model provides helpful answers based on the user's input.

**Response Generation:**
  A function is used to generate responses from OpenAI's GPT models based on the settings provided.

**Customization:**
  Users can adjust parameters such as temperature and maximum tokens for controlling the response style and length.

