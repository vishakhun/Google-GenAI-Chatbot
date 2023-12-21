# Chatbot_Langchain: Chat with Google Gen AI Policy

## Project Overview
The "Chatbot_Langchain" project is designed to create a conversational agent that can discuss Google's Generative AI policies. This is achieved by processing the policies available in PDF format, chunking the text for better handling, embedding the text for semantic search, and finally integrating it into a chatbot framework with memory capabilities.

## Table of Contents
1. Installs, Imports, and API Keys
2. Loading Google Generative AI Policies and Chunking
3. Embedding Text and Storing Embeddings
4. Setting Up Retrieval Function
5. Creating Chatbot with Chat Memory

### 1. Installs, Imports, and API Keys
The first step involves setting up the environment by installing necessary libraries such as LangChain, PyPDF, pandas, and others. An OpenAI API key is also required for accessing certain functionalities.

### 2. Loading Google Generative AI Policies and Chunking
The project starts by loading the Google Generative AI policy document in PDF format. The PDF is then converted into text and split into manageable chunks. This chunking is important for processing and embedding the text later, as it ensures that each piece of text is within a manageable size for analysis.

### 3. Embedding Text and Storing Embeddings
Once the text is chunked, the next step is to embed this text. Embedding converts text into numerical vectors which can be used for semantic searches. These embeddings are stored in a vector database, allowing for efficient retrieval of relevant text chunks based on queries.

### 4. Setting Up Retrieval Function
The project sets up a retrieval function that utilizes the embedded text. This function enables the chatbot to search through the embedded chunks of the policy document to find the most relevant sections in response to user queries.

### 5. Creating Chatbot with Chat Memory
Finally, the chatbot is created using a conversational retrieval chain. This chatbot not only answers queries based on the policy document but also maintains a chat history. This memory feature allows the chatbot to provide context-aware responses and maintain a coherent conversation flow.


