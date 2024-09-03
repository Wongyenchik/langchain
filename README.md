# Langchain
## Langsmith Documentation Rag
### Overview
This project is an application built using Streamlit, showcasing the integration of LangChain's capabilities with Groq and Ollama models for document retrieval and question answering. The application loads documents, splits them into manageable chunks, creates embeddings using the Ollama model, and then stores these embeddings in a vector database. Users can input queries, and the app will retrieve relevant information from the documents and generate responses using the Groq model.

### Features
- Document Loading: Fetches documents from a specified URL using the WebBaseLoader.
- Text Splitting: Documents are split into smaller chunks using the RecursiveCharacterTextSplitter to facilitate better retrieval and processing.
- Embeddings Generation: Utilizes the OllamaEmbeddings to create embeddings for the document chunks.
- Vector Store: Stores the embeddings in a Chroma vector database for efficient similarity search.
- Question Answering: Integrates the ChatGroq model to answer user queries based on the context retrieved from the documents.
- Streamlit Interface: A user-friendly interface for entering queries and viewing responses.
