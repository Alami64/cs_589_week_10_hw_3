# Search and ReRanking System

## Description
This project combines the integration of Weaviate, a vector database, and Cohere, a natural language processing platform, to perform dense retrieval and reranking tasks. 

## Overview

The main components of this project are:

1. `app.py`: The main application file that showcases different examples of dense retrieval and reranking using Weaviate and Cohere.
2. `utils.py`: A utility module containing helper functions for keyword search, dense retrieval, and result printing.
3. `requirements.txt`: A file listing the required Python dependencies for running the project.

## Setup

1. Install the required dependencies by running:
  ```bash
  pip install -r requirements.txt
  ```
2. Set up the necessary environment variables:

    COHERE_API_KEY: Your Cohere API key.
    WEAVIATE_API_KEY: Your Weaviate API key.
    WEAVIATE_API_URL: The URL of your Weaviate instance.

## Examples

The app.py file contains three examples demonstrating different use cases:

    Dense Retrieval:
        Performs a dense retrieval search using Weaviate's vector search capabilities.
        The query is "What is the capital of Canada?".
        The results are printed using the print_result function from utils.py.
    Keyword Search with Reranking:
        Performs a keyword search using Weaviate's BM25 retrieval.
        The query is "What is the capital of Canada?".
        The top 500 results are retrieved and then reranked using Cohere's reranking model.
        The reranked results are printed.
    Improving Dense Retrieval with Reranking:
        Performs a dense retrieval search using Weaviate's vector search capabilities.
        The query is "Who is the tallest person in history?".
        The retrieved results are then reranked using Cohere's reranking model.
        The reranked results are printed.

## Utility Functions

The utils.py module provides the following utility functions:

    keyword_search: Performs a keyword search using Weaviate's BM25 retrieval.
    dense_retrieval: Performs a dense retrieval search using Weaviate's vector search capabilities.
    print_result: Prints the search results with colorful formatting.

## Getting Started

    Make sure you have a Weaviate instance set up and running.
    Obtain the necessary API keys from Cohere and Weaviate.
    Set up the environment variables as mentioned in the Setup section.
    Run the app.py file to see the examples in action:

    ```bash
    python app.py
    ```
