# Conversational RAG with PDF and Chat History

This repository hosts a **Conversational Retrieval-Augmented Generation (RAG)** system using Python and Streamlit.
The application enables users to upload PDF documents and interact with their content via conversational queries, with the context preserved across chat history.

![App Screenshot](docs/app_screenshot.png)

---

## Features

- **PDF Upload**: Users can upload multiple PDFs for document retrieval.
- **Conversational Chat**: Queries and responses maintain context using chat history.
- **Retrieval-Augmented Generation (RAG)**: Combines document embeddings with a Groq-powered LLM for contextual question answering.
- **Streamlit UI**: Simple and intuitive interface for interaction.

---

## Prerequisites

- Python 3.8 or higher
- `pip` (Python package manager)
- [Groq API Key](https://www.groq.com/)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Jimmy70707/rag-chat-pdf.git
   cd rag-chat-pdf
