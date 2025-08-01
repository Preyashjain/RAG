# 🔍 Retrieval-Augmented Generation (RAG) with IBM Granite, HuggingFace, LangChain, Milvus, and Replicate

This project demonstrates how to build a modern RAG (Retrieval-Augmented Generation) pipeline using open-source tools and LLMs. It integrates vector search, prompt chaining, and LLM inference to create a powerful knowledge-aware question-answering system.

## 💡 What is RAG?

RAG (Retrieval-Augmented Generation) is an AI architecture that combines document retrieval with large language models (LLMs) to produce more accurate and grounded answers. Instead of relying solely on pre-trained knowledge, RAG first **retrieves relevant information** from external sources (like vector databases) and then **generates responses** using that context.

## 🧰 Tech Stack

- **🧠 IBM Granite Models (via Hugging Face)**
- **🔗 LangChain** for chaining prompts and managing agents
- **🧮 Milvus** as a vector store for semantic search
- **🧬 Hugging Face Transformers** for tokenization and model support
- **🧪 Replicate** for inference using hosted models
- **📁 Google Colab** for interactive experimentation

## 🚀 Features

- Upload and index documents
- Convert text into embeddings using `langchain_huggingface`
- Store vectors in Milvus
- Retrieve top relevant chunks for any question
- Use an LLM to generate final answer grounded in context

## 📦 Installation (in Google Colab)

```bash
%pip install git+https://github.com/ibm-granite-community/utils \
    transformers \
    langchain_community \
    'langchain_huggingface[full]' \
    langchain_milvus \
    replicate \
    wget
