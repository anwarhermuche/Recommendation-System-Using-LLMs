# LLM Recommendation System using RAG with Query Expansion and Cross-Encoder Re-Ranking
## About the Project
This project presents a Language Large Model (LLM) based recommendation system using Retrieval-Augmented Generation (RAG) with enhancements from Query Expansion and Cross-Encoder Re-Ranking. The system aims to address the limitations of conventional RAG systems, focusing on precision and relevance in document and information retrieval.

## Technical Implementation
The project employs the following models and tools:

- **BERT-based Embeddings**: Utilizing "bert-base-uncased" for generating embeddings, the system leverages this model's proficiency in natural language understanding.

- **Qdrant Vector Database**: Qdrant is used for efficient management and retrieval of vector embeddings, ensuring high-performance similarity searches.

- **Cross-Encoder "cross-encoder/ms-marco-MiniLM-L-6-v"**: This model is employed for re-ranking queries post-expansion, known for its effectiveness in evaluating query-document relevance.

## Project Details
### Query Expansion
The system includes a Query Expansion feature, aiming to align the retrieved documents more accurately with user queries by rewriting and refocusing them. However, in the course of this project, it was observed that Query Expansion did not yield the expected improvements in this context.

### Cross-Encoder Re-Ranking
Post Query Expansion, the Cross-Encoder model is used for re-ranking. This approach offers a detailed analysis of the query-document relationship, yet the additional recommendations from the original method were found to be more sensible and relevant in this specific application.

## Conclusions and Results
The project revealed that despite the higher scores achieved by the example titles (using query expansion) using advanced methods, the best practical results were obtained using the original method without Query Expansion. This highlights an important aspect of AI-driven recommendation systems - the necessity to test and adapt approaches based on specific use cases. While advanced techniques like Query Expansion and Cross-Encoder Re-Ranking hold significant potential, their effectiveness may vary depending on the context.

## Key Takeaway
The outcome of this project serves as a valuable reminder that while technological advancements can provide powerful tools, their application needs to be contextually optimized. It underscores the importance of practical testing and validation in the development of AI systems.
