
# ChatBot: News Research Tool 

The ChatBot is an intuitive news research tool that simplifies information retrieval. Users can enter article URLs and ask questions to quickly obtain relevant insights related to the stock market and financial domain.

<img width="1446" alt="image" src="https://github.com/user-attachments/assets/7f810b3c-3c56-4597-8948-5cd816fe7d40">


## Features

- Load URLs or upload text files containing URLs to fetch article content.
- Process article content through LangChain's UnstructuredURL Loader
- Construct an embedding vector using OpenAI's embeddings and leverage FAISS, a powerful similarity search library, to enable swift and effective retrieval of relevant information
- Interact with the LLM's (Chatgpt) by inputting queries and receiving answers along with source URLs.


## Usage/Examples

1. Run the Streamlit app by executing:
streamlit run main.py

2.The web app will open in your browser.

- On the sidebar, you can input URLs directly.
- Initiate the data loading and processing by clicking "Process URLs."
- Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.
- The embeddings will be stored and indexed using FAISS, enhancing retrieval speed.
- The FAISS index will be saved in a local file path in pickle format for future use.
- One can now ask a question and get the answer based on those news articles

## Project Structure

- main.py: The main Streamlit application script.
- requirements.txt: A list of required Python packages for the project.
- faiss_store_openai: A folder with pickle file to store the FAISS index.
- .env: Configuration file for storing your OpenAI API key.
