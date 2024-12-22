# Uttu baba : News Research Tool 
Uttu baba is a user-frienly news research tool designed for effortless infomation retrieval. Users can input article URls and ask question to recevie relevant insights from the stock market and fincaial domain
![](img.jpg)

## Features 
- Load URLs or upload text files containing URLs to fectech article content.
- Process arcticle content through Langchain's UnstructuredURL Loader
- Construct an embedding vector using llama's Embeddings and leverage FAISS, a powerful similarity search library, to swift and effective retrieval of relevant infomation
- Intracted with LLM by inputting queries and receiving answers along with source URLs.


## Usage/Examples

1. Run the Streamlit app by executing:
```bash
streamlit run main.py

```

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
- faiss_store_openai.pkl: A pickle file to store the FAISS index.
- .env: Configuration file for storing your OpenAI API key.
