# financial-vss
*A detailed set of Google Colab notebooks to handle semantic search in Redis over public financial datasets with [RedisPython](https://redis-py.readthedocs.io/en/stable/index.html), [RedisVL](https://redisvl.com), and [LangChain](https://python.langchain.com/docs/integrations/vectorstores/redis).*

This project is specifically designed for a Google Colab environment to leverage its resources for intensive tasks without local setup hurdles.

___

# Introduction to Redis VSS
[Redis](https://redis.com), widely recognized for its low-latency performance, extends beyond traditional noSQL databases. It's uniquely suited for tasks like caching, session management, job queuing, and JSON storage. With enhanced Search+Query features, Redis emerges as a performant [Vector Database](https://redis.com/solutions/use-cases/vector-database) supporting Vector Similarity Search (VSS) over unstructured data encoded as embeddings.

## Getting Started in Google Colab

Click on one of the three options below to start your journey. It launches a Colab notebook that prepares your environment by cloning the necessary repository artifacts, managing dependencies, and ends with the walkthrough of VSS in Redis.

Select your desired notebook from below:

1. [**RedisPython_VSS**](https://colab.research.google.com/github/Redislabs-Solution-Architects/financial-vss/blob/main/RedisPython_VSS.ipynb): Grasp VSS basics with the standard Redis client.
2. [**RedisVL_VSS**](https://colab.research.google.com/github/Redislabs-Solution-Architects/financial-vss/blob/main/RedisVL_VSS.ipynb): Dive deeper using a dedicated VSS client library.
3. [**LangChain_VSS**](https://colab.research.google.com/github/Redislabs-Solution-Architects/financial-vss/blob/main/LangChain_VSS.ipynb): Wrap up with an integrated approach via LangChain.

## Understanding the Client Ecosystem
Wondering why we have three different clients? Each serves a unique purpose, providing varying abstraction levels. Your choice depends on several factors:

- **Use Cases**: Are you focusing on Pure VSS, RAG, Semantic Caching, etc.?
- **Redis Experience**: How comfortable is your team with Redis clients and commands?
- **Integration Points**: What are your touchpoints with LLMs and Embedding Providers?
- **Performance Demands**: How intensive are your requirements?
- **Configurability**: Do you prefer ease of use or detailed control?

Each notebook explores these considerations, guiding you through making an informed choice for your use case.

## Cautionary Advice
- **Not for Local Use**: This Colab-centric project isn't configured for local environments. Running it outside Colab requires a different setup.
- **Temporary Workspace**: Colab doesn't save your work indefinitely. Download your notebooks or save them to Google Drive to avoid losing progress.
- **Idle Disconnections**: Extended inactivity in Colab can disconnect the runtime, potentially resulting in work loss. Regular saving is your friend!
