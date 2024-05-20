# Complex RAG Flow with Llama 3, watsonx.ai, and Watson Discovery

This code implements a complex Retrieval-Augmented Generation (RAG) flow using Llama 3 from watsonx.ai and IBM Watson Discovery. It allows you to build a sophisticated question-answering system that leverages both curated enterprise knowledge bases and web search results to provide accurate and reliable answers to complex queries.

## Features

- Integration with Llama 3 language model from watsonx.ai for query understanding, document relevance scoring, and answer generation
- Utilization of IBM Watson Discovery for targeted document retrieval from proprietary collections
- Fallback web search functionality for increased coverage and retrieval of information not found in curated knowledge bases
- Query parsing and reformulation techniques to optimize search queries and improve retrieval performance
- Document relevance scoring based on semantic similarity, keyword matching, and entity recognition
- Answer generation with hallucination checking to ensure factual accuracy and grounding in retrieved context
- Parallel processing using joblib for improved efficiency

## Prerequisites

- Python 3.9+
- IBM Watson Discovery service instance
- watsonx.ai account and API credentials
- Required Python packages (see `requirements.txt`)

## Installation

1. Clone the repository: `git clone https://github.com/yourusername/complex-rag-flow.git`
2. Install the required Python packages: `pip install -r requirements.txt`
3. Set up the necessary environment variables (see example.env):
- `WATSONX_URL`: URL for watsonx.ai service
- `WATSONX_APIKEY`: API key for watsonx.ai service
- `WATSONX_INSTANCE_ID`: Instance ID for watsonx.ai service
- `DISCOVERY_PROJECT_ID`: Project ID for IBM Watson Discovery service
- `DISCOVERY_SERVICE_URL`: Service URL for IBM Watson Discovery

Save as `.env`

## Usage

1. Prepare your curated document collections in IBM Watson Discovery.
2. Run the notebook.
