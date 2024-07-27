# RAG Pipeline Documentation

Our Retrieval-Augmented Generation (RAG) pipeline uses a combination of TF-IDF vectorization for retrieval and the Groq language model for generation.

## Retrieval Process

1. The FAQ document is split into questions and answers.
2. Questions are vectorized using TF-IDF vectorization.
3. When a query is received, it is also vectorized using the same TF-IDF vectorizer.
4. Cosine similarity is used to find the best matching question in the FAQ.

## Generation Process

1. If a match is found in the FAQ, the corresponding answer is retrieved.
2. The Groq model is then used to generate a response based on the FAQ answer and the original query.
3. If no match is found in the FAQ, the Groq model generates a response suggesting the user contact customer service.

## Implementation Details

- TF-IDF Vectorization: `sklearn.feature_extraction.text.TfidfVectorizer`
- Similarity Measurement: `sklearn.metrics.pairwise.cosine_similarity`
- Language Model: Groq's `mixtral-8x7b-32768` model

The pipeline ensures that responses are grounded in the provided FAQ while allowing for natural language generation to provide context-appropriate answers.