📝 Description

This workflow builds a Retrieval-Augmented Generation (RAG) assistant that ingests a document from ClickUp, stores it in a Supabase vector database, and enables conversational querying through an AI agent.

When manually triggered, the workflow downloads a PDF file (e.g., a Code of Conduct document) via HTTP, processes it into chunks, generates embeddings using OpenAI, and stores them in Supabase for semantic search.

A chat interface allows users to ask questions about the document. The AI agent retrieves relevant context from the vector store and responds using an OpenAI chat model, while maintaining conversation history with Postgres memory for more coherent multi-turn interactions.


<img width="1669" height="732" alt="image" src="https://github.com/user-attachments/assets/870c2842-f479-4368-9b42-9c708c829c1b" />
