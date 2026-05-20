# AI Customer Support Agent (RAG System)

An AI powered customer support system built with n8n, Gemini, Pinecone, and Postgres memory that automates customer responses using business knowledge.

It retrieves relevant information from a knowledge base, maintains conversation context, and responds like a trained support agent instantly.

## What This System Solves

Most businesses struggle with:

- Repetitive customer questions
- Slow response times
- High support workload
- Scaling support without hiring more staff

This system replaces manual support with an AI agent that understands your business.

## How It Works
1. Knowledge Ingestion Pipeline
Google Docs used as knowledge source
Documents are split into chunks
Converted into embeddings using Gemini
Stored in Pinecone vector database

2. AI Support Agent (Runtime)
User sends a message (Telegram)
AI retrieves relevant context from Pinecone
Gemini generates response using retrieved knowledge
Postgres stores conversation memory
Response is returned instantly

## Architecture
![Architecture](assets/first-workflow.png)

![Architecture](assets/second-workflow-incomplete.png)
