# 🤖 AI Engineering Roadmap MOC

- **Status:** 🧊 Not Started
- **Last Updated:** 2026-08-11
- **Progress:** `📁 03-concepts/` | `🛠️ 04-tools/`

---

## 🧠 Phase 1: AI & LLM Fundamentals
- [ ] [[llm-core-mechanics]] — Tokens, context windows, temperature, and attention mechanisms.
- [ ] [[prompt-engineering]] — Zero-shot, few-shot, chain-of-thought, and system prompts.
- [ ] [[embeddings-and-vectors]] — What high-dimensional vectors are and how semantic search works.

## 🗄️ Phase 2: Vector Infrastructure
- [ ] [[vector-databases]] — Indexing types (HNSW vs. IVF) and distance metrics (Cosine, L2).
- [ ] [[pinecone]] (or [[milvus]] / [[qdrant]]) — Managed standalone vector stores.
- [ ] [[pgvector]] — Storing embeddings directly within your existing Relational Databases.

## 🏗️ Phase 3: RAG (Retrieval-Augmented Generation)
- [ ] [[rag-architecture]] — Naive RAG vs. Advanced RAG workflows.
- [ ] [[data-ingestion-pipelines]] — PDF/text extraction, document chunking, and overlap strategies.
- [ ] [[hybrid-search]] — Combining semantic vector search with keyword-based full-text search.

## 🔌 Phase 4: Frameworks & Orchestration
- [ ] [[langchain]] / [[langgraph]] — Building stateful, graph-based agentic workflows.
- [ ] [[llamaindex]] — Advanced data structuring and ingestion for RAG applications.
- [ ] [[model-providers]] — Navigating [[openai-api]], [[anthropic-api]], and open-source models via [[ollama]].

## 🚀 Phase 5: Production & Operations (LLMOps)
- [ ] [[llm-caching]] — Saving money and reducing latency using tools like [[gptcache]].
- [ ] [[llm-evaluation]] — Measuring system accuracy using frameworks like [[ragas]] or [[truera]].
- [ ] [[semantic-routing]] — Dynamically routing user requests based on intent to save token costs.

---

## 🔬 AI Sandbox Projects
- `05-projects/semantic-search-engine` — Ingesting internal text data and querying via pgvector.
- `05-projects/customer-support-agent` — Building a stateless fallback agent using LangGraph.
