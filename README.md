# GenAI-Document-Summerizer
This project is a Python-based PDF Document Summarizer that implements a Retrieval-Augmented Generation (RAG) pipeline using LangChain, embeddings, and Pinecone.
The system allows users to load a PDF, store its semantic representations in a vector database, and perform context-aware question answering and summarization

**Problem Statement**
Reading and extracting insights from long PDF documents is time-consuming and inefficient.
This project explores how Retrieval-Augmented Generation (RAG) can be used to automate
document summarization and question answering while grounding responses in source content.


**Core Capabilities:**
PDF ingestion with structured text extraction.
Recursive chunking to preserve semantic context across long documents.
Embedding generation using Hugging Face and Pinecone embedding models.
Vector indexing and semantic similarity search using Pinecone.
Retrieval-driven context injection into LLM prompts (RAG).
Document-grounded responses with reduced hallucination.

**How It Works**
Load and parse PDF documents to extract raw text.
Split text into overlapping, semantically meaningful chunks.
Transform text chunks into dense vector embeddings.
Persist embeddings in Pinecone for fast similarity search.
Retrieve the most relevant chunks based on user queries.
Inject retrieved context into the LLM prompt to generate accurate answers and summaries.
