# Multi AI Agent with RAG and WikiSearch

This project demonstrates the integration of multiple AI agents using Retrieval-Augmented Generation (RAG) and WikiSearch functionalities, along with Cassandra for data storage and retrieval. It leverages Llama 3.1 for natural language processing and "all-MiniLM-L6-v2" for generating embeddings.

## Overview

This project, implemented in a Jupyter Notebook, showcases how to:

*   Connect to Cassandra.
*   Load and process data from web pages using `WebBaseLoader`.
*   Convert text to vectors using the "all-MiniLM-L6-v2" Hugging Face embedding model.
*   Perform document retrieval and question routing using LangChain and related libraries.
*   Generate human-like responses using the Llama 3.1 LLM via GROQ.

## Features

*   **Cassandra Integration:** Connects to Cassandra for storing and retrieving document embeddings.
*   **LangChain:** Utilizes LangChain for web page loading, text splitting, embedding, and vector store operations.
*   **WebBaseLoader:** Uses `WebBaseLoader` to efficiently load content from web pages.
*   **Hugging Face Embeddings:** Employs the "all-MiniLM-L6-v2" model for generating high-quality text embeddings.
*   **Llama 3.1 with GROQ:** Integrates the Llama 3.1 LLM using GROQ for refined, human-like responses.
*   **WikiSearch:** Integrates the Wikipedia API for answering questions not related to stored documents.
*   **Query Routing:** Routes user queries to either the Cassandra vector store or WikiSearch based on relevance.
