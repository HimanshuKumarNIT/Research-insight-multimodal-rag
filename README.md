# Research Insight – Multimodal RAG PDF QA

This project is a small research assistant that can read a PDF and answer questions from it. It works on text, tables, and images inside the document using a multimodal RAG pipeline. The main goal was to build something practical that can understand research papers better than normal text-only systems.

# What the system does
  
.Extracts text, tables, and images from a PDF
.Creates short summaries and embeddings for better retrieval
.Stores everything using a multi-vector setup (summaries + raw content)
.Retrieves the most relevant pieces based on the user’s question
.Uses Gemini Vision to combine text + images and generate the final answer
.The idea is to get answers that are grounded in the actual PDF content.

# Tech Used

Gemini Pro & Gemini Pro Vision
LangChain
ChromaDB
Unstructured (for PDF parsing)
Streamlit
Python

# How it works 

You upload a PDF
The system breaks it into texts, tables, and images
Summaries → Embedded into Chroma
Raw content → Stored for retrieval
The retriever finds the most relevant part for your question
Gemini Vision reads that text + image context and answers your question

# Why I built this

I wanted to learn how multimodal RAG works end-to-end and how LLMs can handle PDFs that mix text, tables, and charts. This project helped me understand vector stores, embeddings, multimodal prompts, and chaining in LangChain.
