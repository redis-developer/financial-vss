# financial-vss
*A detailed set of Google Colab notebooks to handle semantic search in Redis over public financial datasets with RedisPython, RedisVL, and LangChain.*

This project is specifically designed for a Google Colab environment to leverage its resources for intensive tasks without local setup hurdles. We integrate several technologies, showcasing the versatility and power of Redis for handling complex tasks such as **Vector Similarity Search (VSS)** in modern AI workloads.

<a href="https://colab.research.google.com/github/Redislabs-Solution-Architects/financial-vss/blob/main/SetupColabEnvironment.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

___

# Introduction to Redis VSS
[Redis](https://redis.com), widely recognized for its low-latency performance, extends beyond traditional noSQL databases. It's uniquely suited for tasks like caching, session management, job queuing, and JSON storage. With enhanced Search+Query features, Redis emerges as a performant [Vector Database](https://redis.com/solutions/use-cases/vector-database) supporting Vector Similarity Search (VSS) over unstructured data encoded as embeddings.

# Getting Started in Google Colab
## Step 1: Launch the Setup Notebook
Click on the `Open in Colab` badge above to start your journey. It launches a Colab notebook that prepares your environment by cloning the necessary repository and managing dependencies. This step is crucial, and the rest of the project hinges on this setup.

## Step 2: Execute the Setup
Once in Google Colab, initiate the notebook execution:

1. Click on the 'Runtime' tab in the top menu.
2. Select 'Run all' from the dropdown.
3. Confirm the action.

This process clones the repository, sets up your environment, and ensures you're ready to tackle VSS with Redis! It might take a few minutes, so now's a good time for a cup of coffee.

## Step 3: Navigate the Project Structure
Post-setup, all project files reside in your Google Colab environment. Use the file navigation on the left 📁 to find the `financial-vss`` directory. This repository is your command center for the next steps.

## Step 4: Dive into VSS Notebooks
With the environment primed, proceed to the core of the project: the VSS notebooks. Open them from the `financial-vss/notebooks` directory and run them as you did with the setup notebook.

Remember, start with the [SetupColabEnvironment](SetupColabEnvironment.ipynb) notebook. It's the gateway to the following:

1. [RedisPython_VSS](notebooks/RedisPython_VSS.ipynb): Grasp VSS basics with the standard Redis client.
2. [RedisVL_VSS](notebooks/RedisVL_VSS.ipynb): Dive deeper using a dedicated VSS client library.
3. [LangChain_VSS](notebooks/LangChain_VSS.ipynb): Wrap up with an integrated approach via LangChain.

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

### Testing Notebooks (Not Required)
For notebook tests, set your OpenAI API key and ensure Python requirements are met:

```bash
$ export OPENAI_API_KEY="..."
$ ./test-notebooks.sh
```
