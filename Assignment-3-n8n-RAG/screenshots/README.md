# Screenshots – n8n + RAG Credit Appraisal Chatbot

This folder contains screenshots documenting the development, configuration, execution, and testing of the n8n-based RAG chatbot.

The screenshots provide visual evidence of the complete workflow, from document ingestion and embedding generation to vector retrieval and final chatbot responses.

---

## 1. Workflow Overview

Screenshot showing the complete n8n workflow, including:

- Document ingestion pipeline
- Google Drive document retrieval
- Default Data Loader
- Ollama embeddings
- Simple Vector Store
- Chat Trigger
- AI Agent
- Ollama Chat Model
- Simple Memory
- Vector Store Tool

**File:** `01_workflow_overview.png`

---

## 2. Google Drive – Knowledge Base

Screenshot showing the Google Drive / Download File configuration used to retrieve the Credit Appraisal RAG Knowledge Base.

**File:** `02_google_drive.png`

---

## 3. Default Data Loader

Screenshot showing the configuration used to process the uploaded knowledge-base document.

Key configuration demonstrated:

- Type of Data: Binary
- Mode: Load All Input Data
- Data Format: Automatically Detect by Mime Type
- Text Splitting: Simple

**File:** `03_data_loader.png`

---

## 4. Ollama Embeddings

Screenshot showing the embedding configuration used during document ingestion.

**Embedding Model:**

```text
mxbai-embed-large:latest
