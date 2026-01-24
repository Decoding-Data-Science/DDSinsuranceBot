# DDS Insurance Q&A — RAG Assistant (Pinecone + OpenAI + Gradio)

A beginner-friendly, **document-grounded** Insurance Q&A bot you can replicate and deploy on **Hugging Face Spaces**. It answers **only** from your uploaded insurance documents using **LlamaIndex + Pinecone (serverless) + OpenAI**, with a simple, polite system prompt.

---

## Summary

- **Grounded answers only**: if it’s not in your docs → the bot politely says it can’t find it.
- **Simple UI**: FAQ dropdown + free-text question input.
- **Easy replication**: clean, minimal structure for beginners.
- **Deployable**: designed for Hugging Face Spaces.

---

## What You’ll Get

- A deployed **Space URL** you can share.
- **Grounded answers** (no docs → polite refusal).
- A simple Gradio UI:
  - FAQ dropdown
  - Free-text question box
  - Centered header logo (`data/dds_logo.png`)
- Beginner-friendly defaults + clear error messages.

---

## Features

- **RAG-only answers** (strictly from your documents).
- **Pinecone serverless index**:
  - `aws/us-east-1`
  - `cosine`
  - `1536-dim`
- **OpenAI models**
  - Embeddings: `text-embedding-3-small`
  - LLM: `gpt-4o-mini`
- **Gradio UI** with required logo: `data/dds_logo.png`
- Beginner-friendly UX and troubleshooting.

---

## Repository Structure

```text
.
├─ data/                     # Your insurance docs + required logo
│  └─ dds_logo.png           # REQUIRED (shown in header)
├─ app.py                    # Main app: indexing + query + Gradio UI
├─ requirements.txt          # Dependencies
└─ README.md                 # This file
