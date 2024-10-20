# RAG_Assistant_for_Pathway_PS

This is a repository that contains a Colab notebook for an RAG-based assistant, with all reference links converted to PDFs (and later stored in a vector-embedded database).

## Instructions

This repository contains:
- A Colab notebook
- A database (in PDF format) containing all the refrence links coverted to pdfs provided in the ps.

### To run this:
1. Copy the notebook to Colab.
2. Paste the relevant PDFs into the runtime file option.


An embedded vector database will be uploaded soon. For now, all PDFs should be uploaded manually in the runtime.

## A simple use case is as follows:

**Query**: What is the problem statement?

**Response**: "The problem statement is to create an Agentic RAG system using Pathway that autonomously retrieves, analyzes, and synthesizes information from multiple data sources. The system should dynamically decide the best approach for handling complex queries, utilizing techniques like corrective RAG and multi-agent collaboration to provide accurate responses."


### Data Flow

```plaintext
Query ---------------------------> Data Augmentation ------> LLM ---------> Final Response
  ^                                     ^
  |                                     |
Search Engine --> Vector Database --> Retrieved Data <--- Embedding Pipeline <--- Database

