# financial-vss
*A detailed set of notebooks to handle semantic search in Redis over public financial docs.*

Redis is popularily used as a low-latency, noSQL database for a variety of tasks like caching, session management, job queuing, and even document (JSON) storage. However, extending it's native Search+Query features, Redis is often used as a Vector Database supporting Vector Similarity Search (VSS) for GenAI + LLM workloads.

## Notebooks
Below are a series of notebooks that demonstrate the full capabilities of Redis as a vector database and highlight the various integrations and clients in the AI ecosystem.

The first notebook, [DataPrepLangchain](DataPrepLangChain.ipynb), is required in order to run the following 3 VSS notebooks. It handles data preparation and dependency installation. Each notebook below focuses on data loading, indexing, configuration options, and search techniques:

- [RedisPython_VSS](RedisPython_VSS.ipynb): VSS Basics with the standard Redis client
- [RedisVL_VSS](RedisVL_VSS.ipynb): Use a dedicated VSS client lib
- [LangChain_VSS](LangChain_VSS.ipynb): Wrapping it all with LangChain

## Why 3 different clients?
The choice of client here depends on your team's:
- Use Cases (Pure VSS, RAG, Semantic Caching, etc)
- Comfort & Familiarity with Redis clients and commands
- Integration touch points (LLMs, Embeddings Providers)
- Performance requirements
- Desired configurability / flexibility

Redis is striving to provide a tool to access Redis as a vector db that fits you and your teams needs.

## Running Notebook Tests
Set your openai api key (make sure python requirements are also installed). Run:
```bash
$ export OPENAI_API_KEY="..."
$ ./test-notebooks.sh
```
