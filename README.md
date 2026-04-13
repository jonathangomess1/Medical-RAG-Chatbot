# Medical-RAG-Chatbot
This chatbot uses a Retrieval-Augmented Generation (RAG) approach, which retrieves the 2 most 
relevant text chunks from PDFs via semantic search (MiniLM embeddings + ChromaDB) and 
combines them with conversation history to build the LLM prompt. The Falcon3-3B model then 
generates the answers. Some key design choices include limiting context to the top two relevant 
chunks for efficiency, splitting PDFs into overlapping text chunks to preserve information, and 
maintaining a stateful chat history to provide context-aware responses.
