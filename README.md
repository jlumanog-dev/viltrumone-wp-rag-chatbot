# viltrumone-wp-rag-chatbot

This is a custom RAG chatbot for a WordPress Ecommerce shop. 

It contains 3 main workflows at the moment: The first is the ingestion workflow where the user uploads a new document to be mapped into vector embeddings and stored in a vector database index via Pinecone. The second is the Query workflow that incoming user queries via webhooks and AI agent with access to relevant tools to handle user queries. The third is the Agent telemetry and cost tracker workflow, which is a subworkflow executed at the end of the query workflow to log relevant data for each query and response.

Key features:
- Logging sessions, query and response, latency, and total cost per token input and output.
- Chat memory
- Tool calling: Agent accessing the WooCommerce for product and order details to answer relevant customer queries.
- Escalation measures, issuing a new ticket and notify team via gmail instead of making the agent guess further and hallucinate.

<img width="1665" height="778" alt="image" src="https://github.com/user-attachments/assets/0af6af94-48c2-44a6-9777-7223f5abb720" />

<img width="1545" height="681" alt="image" src="https://github.com/user-attachments/assets/4d4dbe07-7e13-4df5-b353-c6170d1c3c7f" />


