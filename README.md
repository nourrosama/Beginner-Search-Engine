# Beginner-Search-Engine
# Document Search Engine using MID Dataset

## Overview

This project implements a document search engine using the MID dataset, leveraging various information retrieval and natural language processing techniques. The project involves data preprocessing, indexing, query processing, and query expansion using TF-IDF, BM25, and word embeddings.

## Tools and Technologies

- **Languages:** Python
- **Libraries:** PyTerrier, Pandas, NLTK, Gensim, Gradio
- **Data Source:** MID dataset
- **Frameworks:** PyTerrier

## Project Steps

### 1. Data Collection

- **Load CISI Dataset:** The dataset is extracted from a zip file and includes documents, queries, and relevance judgments.
- **Read Documents:** Extract text from the MID.ALL file.
- **Read Queries:** Extract query text from the MID.QRY file.
- **Read Qrels:** Extract relevance judgments from the MID.REL file.

### 2. Data Preprocessing

- **Tokenization:** Split text into tokens.
- **Stopword Removal:** Remove common stopwords.
- **Stemming:** Reduce words to their root forms.
- **Cleaning:** Remove special characters, tabs, and extra white spaces.

### 3. Indexing

- **Index Documents:** Use PyTerrier’s DFIndexer to create an index of the preprocessed documents.

### 4. Query Processing

- **TF-IDF Model:** Implement TF-IDF retrieval model to process and rank documents based on the query.

### 5. Query Expansion

- **Word2Vec Model:** Train a Continuous Bag of Words (CBOW) model to create word embeddings.
- **BM25 Model:** Implement BM25 retrieval model for initial ranking.
- **RM3 Query Expansion:** Expand the query using RM3 method based on the initial BM25 results.
