# RAG-Mistral7b

## Project Description
This repository contains the implementation of the Retrieval Augmented Generation (RAG) model, using the newly released Mistral-7B-Instruct-v0.1 as the Language Model, SentenceTransformers for embedding, and llama-index for data ingestion, vectorization, and storage. The model has been implemented in a Google Colab notebook, optimized for a v100 instance.

The implementation focuses on querying data from Amazon’s Annual Report for the fiscal year ended December 31, 2022. This enables the extraction of insightful information and knowledge encapsulated in the fiscal documents.

## Contents
- `RAG_testing_mistral7b.ipynb` : The main Google Colab notebook containing the entire implementation and execution details.

## Prerequisites
- Google Colab with v100 instance.
- Knowledge on RAG, SentenceTransformers, and Mistral 7B models.
- Access token for HuggingFace (read)

## Implementation Details
### 1. **Mistral 7B Model (LLM)**
   This implementation utilizes Mistral 7B as the Large Language Model to generate human-like, coherent responses based on the retrieved documents.

### 2. **SentenceTransformers (Embedding Model)**
   SentenceTransformers is used to create embeddings for the sentences, enabling efficient and semantic similarity search among them. **all-mpnet-base-v2** pretrained model was used as it had the best performance. 

### 3. **llama-index (Data Ingestion, Vectorization, and Storage)**
   llama-index is employed for ingesting and vectorizing the dataset and for storing the vectorized representations of the data.

### 4. **Data Source**
   The data queried in this implementation is sourced from Amazon’s Annual Report for the fiscal year ended December 31, 2022. 


## Acknowledgments
- The entire team at Mistral for the powerful language model.
- SentenceTransformers for the efficient embedding model.
- llama-index for data ingestion and vectorization.
- Amazon for the annual report data.
