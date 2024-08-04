# <font color = 'green'> 📚 AI Chatbot for Citation of Custom PDFs, Reports, and Guidelines

Unleash the power of instant information retrieval with our state-of-the-art AI Chatbot, designed to provide quick answers and references from a curated directory of PDFs, including essential documents like WHO recommendations. This innovative repository utilizes **Retrieval-Augmented Generation (RAG)** to assist researchers, policymakers, and the public in navigating extensive documents efficiently.

![AI Chatbot Demo](https://github.com/MaxMLang/RAG-nificent/raw/master/assets/demov0.0.2.gif)

## Features:

- **💬 Conversational Interface**  
  Engage with the system using natural language queries to receive responses directly sourced from the PDFs.

- **🔗 Direct Citation**  
  Every response includes a direct link to the source PDF page, ensuring traceability and verification.

- **📄 PDF Directory**  
  Access a predefined set of key PDF documents, currently including WHO recommendations on major health topics such as schistosomiasis and malaria.

## Available Models:

- **llama-3.1-8b-instant**: Experience instant, efficient responses with this model optimized for quick interactions.

- **llama-3.1-70b-versatile**: Utilize this versatile model for a wide range of complex language tasks with high accuracy.

- **gpt-3.5-turbo**: Engage with advanced, human-like interactions suitable for varied conversational tasks.

- **llama3-70b-8192**: Enjoy high-end performance with this large-scale model, ideal for deep learning insights.

- **llama3-8b-8192**: Harness robust capabilities with this more accessible version of Llama3, perfect for a wide range of AI applications.

- **mixtral-8x7b-32768**: Leverage the power of ensemble modeling with Mixtral's extensive capacity for nuanced understanding and response generation.

- **gemma-7b-it**: Explore specialized interactions and tech-focused solutions with Gemma, tailored for IT and technical content.

## How It Works:

The application utilizes a combination of OpenAI embeddings, Pinecone vector search, and a conversational interface to provide a seamless retrieval experience. When a query is made, the system:

1. Converts the query into embeddings.
2. Searches for the most relevant document sections using Pinecone's vector search.
3. Returns the answer along with citations and links to the source documents.

## Setup Instructions:

### Clone the Repository

```git clone https://github.com/yourusername/RAG-nificent.git```

#### Install Dependencies

```pip install -r requirements.txt```

#### Set Environment Variables

Create a .env file (see .env.example for reference) with the following variables:

```
PINECONE_INDEX_NAME
PINECONE_NAME_SPACE
OPENAI_API_KEY
PINECONE_API_KEY
GROQ_API_KEY
```

#### Create a Pinecone Index
Create a Pinecone index with the same name as `PINECONE_INDEX_NAME`. Set it up with `dimensions=1536` and `metric=cosine`.
#### Data Ingestion
Place your PDFs in the pdf_data directory and run data_ingestion.py.
Run the Application
```chainlit run src/app.py```


### Valuable Resources:
1. Pinecone Documentation: [Learn more about Pinecone](https://github.com/MaxMLang/RAG-nificent/blob/master/pinecone.io)
2. OpenAI API Documentation: [Explore OpenAI API](https://github.com/MaxMLang/RAG-nificent/blob/master/pinecone.io)

### <font color = 'green'> Get Started Today!

Harness the power of AI to streamline your research and information retrieval processes. Dive into the future of document citation and retrieval with our AI Chatbot! 🚀
