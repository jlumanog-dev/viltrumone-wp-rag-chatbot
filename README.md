# viltrumone-wp-rag-chatbot

This is a custom RAG chatbot for a WordPress Ecommerce shop. 

It contains 2 main workflows at the moment: The first is he ingestion workflow where the user uploads a new document to be mapped into vector embeddings and stored in a vector database index using Pinecone. The second is the Query workflow that incoming user queries via webhooks and AI agent with access to relevant tools to handle user queries.

List of additional main features yet to be implemented:
- Logging every conversation
- Chat memory
- Tool calling: Connect agent to the store to answer account questions
- Implementing escalation measures instead of making the agent guess further and hallucinate
- Immplement a separate evaulation rnner workflow with golden question sets to test the quality of agent response