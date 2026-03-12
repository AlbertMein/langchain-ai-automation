# langchain-ai-automation

LangChain-based agents, chains, and RAG pipelines for automating tasks that need language understanding.

## What this covers

- **Agents** — LangChain agents with custom tools for web research, data analysis, and code execution
- **Chains** — LCEL-based chains for multi-step workflows (summarization, extraction, classification)
- **RAG pipelines** — Document ingestion, chunking, vector storage, and retrieval with FAISS/Pinecone
- **Prompt management** — Reusable prompt templates with few-shot examples and output parsers

## Stack

- Python 3.10+
- LangChain / LangGraph
- OpenAI, Anthropic, Google AI
- FAISS, Pinecone, Weaviate
- Pydantic, pytest, ruff

## Structure

```
agents/          # Agent implementations (one per use case)
chains/          # LCEL chain definitions
rag/             # Loaders, splitters, retrievers, vector store configs
tools/           # Custom tools for agents
prompts/         # Prompt templates and system messages
tests/           # Mirrored test structure
examples/        # Usage examples and notebooks
```

## Setup

```bash
pip install -e .
cp .env.example .env  # add your API keys
pytest                 # run tests
```

## License

MIT
