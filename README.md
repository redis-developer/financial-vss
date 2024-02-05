<div align="center">
    <div style="display: inline-block; text-align: center; margin-bottom: 10px;">
        <span style="font-size: 36px;"><b>Redis Vector Search: Financial Examples</b></span>
        <br />
    </div>
    <br />
</div>


<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Language](https://img.shields.io/github/languages/top/Redislabs-Solution-Architects/financial-vss)
![GitHub last commit](https://img.shields.io/github/last-commit/RedisVentures/RedisVL)

</div>

<div align="center">
<div display="inline-block">
    <a href="https://github.com/RedisVentures/redisvl"><b>Home</b></a>&nbsp;&nbsp;&nbsp;
    <a href="https://www.redisvl.com"><b>Documentation</b></a>&nbsp;&nbsp;&nbsp;
    <a href="https://github.com/RedisVentures"><b>More Projects</b></a>&nbsp;&nbsp;&nbsp;
  </div>
    <br />
</div>




*A detailed set of Google Colab notebooks to teach semantic search in Redis over public financial 10k documents with different Redis clients and integrations including: [redis-py](https://redis-py.readthedocs.io/en/stable/index.html), [redisvl](https://redisvl.com), and [langchain](https://python.langchain.com/docs/integrations/vectorstores/redis).*

# ⚡ Introduction to Vector Search in Redis
[Redis](https://redis.com), widely recognized for its low-latency performance, extends beyond traditional noSQL databases. It's uniquely suited for tasks like caching, session management, job queuing, and JSON storage. With enhanced Search+Query features, Redis emerges as a performant [Vector Database](https://redis.com/solutions/use-cases/vector-database) supporting Vector Search over unstructured data encoded as embeddings.

## 📚 Getting Started in Google Colab

Click on one of the three notebook options below to start your journey. It launches a Colab notebook that prepares your environment by cloning the necessary repository artifacts, managing Python dependencies, and ends with an end-to-end walkthrough of vector search in Redis.

Select your desired notebook tutorial from below:

| # | Notebook | Description | Documentation |
|---|----------|-------------|---------------|
| 1 | [**redis-py-01**](https://colab.research.google.com/github/Redislabs-Solution-Architects/financial-vss/blob/main/redis-py-01.ipynb) | Grasp VSS basics with the standard Redis client. | View Docs |
| 2 | [**redisvl-02**](https://colab.research.google.com/github/Redislabs-Solution-Architects/financial-vss/blob/main/redisvl-02.ipynb) | Dive deeper using a dedicated VSS client library. | View Docs |
| 3 | [**langchain-03**](https://colab.research.google.com/github/Redislabs-Solution-Architects/financial-vss/blob/main/langchain-03.ipynb) | Wrap up with an integrated approach via LangChain. | View Docs |


## 🛠️ Understanding the Client Ecosystem
Wondering why there are multiple clients? Each serves a unique purpose, providing varying abstraction levels. Your choice depends on several factors:

- **Use Cases**: Are you focusing on pure vector search, RAG, or other tasks like LLM semantic caching?
- **Redis Experience**: How comfortable is your team with Redis clients and commands?
- **Integration Points**: What are your touchpoints with LLMs and Embedding Providers?
- **Performance Demands**: How intensive are your performance requirements?
- **Configurability**: Do you prefer ease of use or fine-grained control?

Each notebook explores these considerations, guiding you through making an informed choice for your use case.

## ⚠️ Cautionary Advice
- **Not for Local Use**: This Colab-centric project isn't configured for local environments. Running it outside Colab requires a different setup.
- **Temporary Workspace**: Colab doesn't save your work indefinitely. Download your notebooks or save them to Google Drive to avoid losing progress.
- **Idle Disconnections**: Extended inactivity in Colab can disconnect the runtime, potentially resulting in work loss. Regular saving is your friend!
