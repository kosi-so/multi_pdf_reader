## Overview
This application allows users to upload one or multiple PDF documents, process their content, and then ask questions about the documents. The app uses Google Generative AI and LangChain to answer user questions based on the content of the uploaded PDFs.

Key functionalities include:
-Extracting text from one or multiple PDF files.  
-Splitting the extracted text into manageable chunks for better processing.  
-Embedding the text using Google Generative AI Embeddings.  
-Creating a conversational chain that allows users to ask questions about the uploaded documents.

## Features
Upload Multiple PDFs: Users can upload one or more PDF files.
Text Extraction: The app extracts text from the uploaded PDFs using PyPDF2.
Text Chunking: Large text content is split into smaller chunks using LangChain's RecursiveCharacterTextSplitter.
Vector Store Creation: The extracted text chunks are embedded and stored in a FAISS vector store for fast similarity search.
Question Answering: Users can ask questions related to the uploaded PDFs, and the app will provide answers based on the document's content using Google's Generative AI.

## Requirements
Libraries
streamlit: For building the web application interface.
PyPDF2: For reading and extracting text from PDF files.
langchain: For handling AI-based processing, text chunking, and conversational chains.
google-generativeai: For embedding the text and interacting with Google's Generative AI models.
faiss: For efficient similarity search over the document content.
dotenv: For loading environment variables, including your Google API key.
