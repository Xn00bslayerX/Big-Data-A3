# Big-Data-A3

This assignment is focused on building a simple retrieval augmented generation (RAG) system using the Chroma vector database and OpenAI's language models. The goal is to create a system that can answer questions about a collection of documents by retrieving relevant chunks of text and using them to generate answers. The assignment is structured as follows:

1. **Data Preparation**: We will start by loading a collection of documents, cleaning the text, and chunking it into smaller pieces that can be embedded and stored in the vector database.
2. **Embedding and Storage**: We will use a pre-trained embedding model to convert the chunks of text into vector representations and store them in the Chroma vector database along with metadata about the source document.
3. **Querying and Retrieval**: We will implement a function that takes a user query, converts it into an embedding, and retrieves the most relevant chunks of text from the vector database based on cosine similarity.
4. **Answer Generation**: We will use OpenAI's language models to generate answers to the user queries based on the retrieved chunks of text. We will also include a system prompt to guide the model in generating concise and accurate answers based on the provided information.
5. **Evaluation**: Finally, we will evaluate the performance of our RAG system by testing it with a set of queries and analyzing the quality of the generated answers. We will also experiment with different models and chunking strategies to see how they affect the results.

# Setup

Install python, then Run `pip install -r requirements.txt` to set up the environment and load the necessary libraries.
Configure your API key by setting the `SATORI_API_KEY` environment variable to your API key. This will allow you to access the language models for answer generation. Without an API key, you will only go up to the chunk embedding and storage steps, but you won't be able to generate answers to queries.