# viltrumone-wp-rag-chatbot

This is a custom RAG chatbot for a WordPress Ecommerce shop. 

It contains 3 main workflows at the moment: The first is the ingestion workflow where the user uploads a new document to be mapped into vector embeddings and stored in a vector database index via Pinecone. The second is the Query workflow that incoming user queries via webhooks and AI agent with access to relevant tools to handle user queries. The third is the Agent telemetry and cost tracker workflow, which is a subworkflow executed at the end of the query workflow to log relevant data for each query and response.

Key features:
- Logging sessions, query and response, latency, and total cost per token input and output.
- Chat memory
- Tool calling: Agent accessing the WooCommerce for product and order details to answer relevant customer queries.
- Escalation measures, issuing a new ticket and notify team via gmail instead of making the agent guess further and hallucinate.
