## stores pdf in vector database and retrieves relevant information to answer user queries 

Uses FAISS and huggingface embeddings to embed and store in a vector database

First, creates a document chain to use all the documents to answer the user query, this method is time consuming since all documents are used so we use a more efficient method. 

Second, it creates a retrieval chain using custom made prompt template, LLAMA2 llm model from OLLAMA, and documents for context. this only fetches the relevant documents instead of all the documents and answers the query
