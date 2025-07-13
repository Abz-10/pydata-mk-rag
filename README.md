# pydata-mk-rag
---
# PyData Milton Keynes 2025: Building RAG Chatbots with LangChain and Gemini

Welcome to the PyData Milton Keynes 2025 workshop on building advanced AI chatbots! This repository contains the Jupyter Notebook and all the necessary files for our hands-on session.

In this workshop, we will explore the exciting world of Large Language Models (LLMs) and build a chatbot that can answer questions about documents it has never seen before. We'll start with a basic conversational AI and then level up by implementing a **R**etrieval-**A**ugmented **G**eneration (RAG) pipeline.

## What You'll Learn

By the end of this session, you will understand and be able to:

-   **Interact with LLMs**: Use the `langchain` library to communicate with powerful models like Google's Gemini.
-   **Manage Conversations**: Structure and maintain conversational history to build stateful chatbots.
-   **Understand LLM Limitations**: See firsthand the challenges of knowledge cutoffs and "hallucinations."
-   **Implement RAG**: Learn the theory and practice of Retrieval-Augmented Generation to ground your LLM in factual, external data.
-   **Build a Knowledge Base**: Use `ChromaDB` and `Hugging Face` sentence transformers to load, split, and embed a PDF document into a searchable vector store.
-   **Create a Document-Aware Chatbot**: Combine retrieval and generation to build a bot that can accurately answer questions based on the contents of your private documents.

## Requirements

### Libraries

You'll need a few Python libraries to get started. You can install them all with the following command:

```bash
pip install -qU \
    dotenv \
    sentence-transformers \
    langchain \
    langchain-community \
    langchain-chroma \
    langchain-google-genai \
    langchain-huggingface \
    pypdf
```

### API Keys

This notebook uses the Google Gemini API. You will need a **Google API Key** to run the cells.

-   You can get your free API key from [Google AI Studio](https://aistudio.google.com/apikey).

The notebook is configured to securely ask for your API key if it's not set as an environment variable.

## How to Run This Workshop

Follow these steps to get set up:

1.  **Clone or Download the Repository**
    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  **Set Up a Virtual Environment (Recommended)**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the Dependencies**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: You can create a `requirements.txt` file with the packages listed above for easier installation.)*

4.  **Launch Jupyter**
    ```bash
    jupyter notebook
    ```
    Or, if you prefer JupyterLab:
    ```bash
    jupyter lab
    ```

5.  **Open and Run the Notebook**
    -   Open the `rag-chatbot.ipynb` file.
    -   Run the cells sequentially from top to bottom.
    -   If you have not created a `.env` file, when prompted, enter your Google API key.

## File Structure

-   `rag-chatbot.ipynb`: The main Jupyter Notebook for the workshop.
-   `pdfs/2501.17805v1.pdf`: The source document we will use to build our RAG pipeline's knowledge base.
-   `README.md`: This file!

---

We're excited to have you here and can't wait to see what you build. Let's get started
