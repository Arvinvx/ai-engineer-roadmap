# Layer 2 — AI Engineering Core

**Course:** [Scrimba AI Engineer Path](https://scrimba.com/the-ai-engineer-path-c02v)  
**Timeline:** Aug 2026 – Oct 2026  
**Goal:** Build real AI-powered products using LLMs, embeddings, and retrieval pipelines.

---

## What You Learn

### 1. Working with LLM APIs

The foundation of modern AI engineering — calling language models and getting useful output.

- OpenAI API: `chat/completions`, `embeddings`, `images`
- Anthropic API: Claude models, messages format
- API authentication, rate limits, and cost management
- Token counting and context window limits
- Streaming responses for real-time output
- Handling API errors gracefully — retries, fallbacks
- Switching between models and providers

**Why it matters:** Every AI product starts here. Understanding the API layer deeply — not just "send prompt, get response" — is what separates engineers from power users.

---

### 2. Prompt Engineering

How you write prompts determines the quality of everything downstream.

- System prompts vs user messages — how the roles work
- Few-shot prompting: teaching the model by example
- Chain-of-thought prompting: making the model reason step by step
- Temperature and top-p — controlling randomness
- Structured output: forcing JSON, lists, and schemas
- Prompt chaining: breaking complex tasks into smaller steps
- Common failure modes: hallucination, over-refusal, drift
- Evaluating prompt quality systematically

**Why it matters:** A well-crafted prompt is often the difference between a product that works and one that doesn't. This is a core engineering skill, not a soft one.

---

### 3. Embeddings and Semantic Search

How AI understands meaning, not just keywords.

- What embeddings are: turning text into vectors
- Cosine similarity — measuring meaning distance
- OpenAI `text-embedding-ada-002` and newer models
- Building a semantic search engine from scratch
- When semantic search beats keyword search (and when it doesn't)
- Chunking strategies: how to split documents for embedding
- Embedding different content types: text, code, structured data

**Why it matters:** Embeddings are the backbone of every RAG system, recommendation engine, and semantic search product. You can't build serious AI features without understanding them.

---

### 4. Retrieval-Augmented Generation (RAG)

The dominant pattern for grounding LLMs in real, up-to-date data.

- The RAG architecture: retrieve → augment → generate
- Vector databases: Pinecone, Weaviate, Chroma, pgvector
- Indexing a document corpus: chunk, embed, store
- Query-time retrieval: embed the question, find nearest chunks
- Injecting retrieved context into the prompt
- Handling context window limits with smart truncation
- Reranking: scoring retrieved chunks for relevance
- Hybrid search: combining semantic + keyword retrieval
- Evaluating RAG quality: faithfulness, relevance, groundedness

**Why it matters:** RAG is how you build AI products that know things the model wasn't trained on — your docs, your users' data, your company's knowledge base. It's the most-used pattern in production AI today.

---

### 5. Building AI Pipelines

Connecting multiple AI steps into reliable, production-ready flows.

- LangChain fundamentals: chains, agents, tools, memory
- Multi-step pipelines: classify → retrieve → generate → format
- Memory patterns: conversation history, summarization, entity tracking
- Tool use / function calling: letting the model take actions
- Agents: when to let the model decide the next step
- Streaming in pipelines — keeping responses fast
- Handling failures: retries, fallbacks, graceful degradation
- Observability: logging inputs, outputs, and latency at every step

**Why it matters:** Real AI features aren't single API calls — they're pipelines. Knowing how to compose, debug, and monitor multi-step AI flows is what makes you a product-level AI engineer.

---

### 6. AI-Powered Product Patterns

The recurring architectures behind real AI products.

- Document Q&A systems — upload docs, ask questions
- AI chat interfaces with persistent conversation history
- Summarization pipelines for long-form content
- Classification and routing: triage tickets, categorize content
- Code assistants: context-aware autocomplete and explanation
- Content generation with quality controls
- AI-assisted search: query expansion, result reranking

**Why it matters:** These are the patterns you'll reach for again and again. Knowing them lets you scope, estimate, and build AI features faster.

---

## Skills Unlocked After This Layer

By the end of Layer 2, you can:

- Integrate any LLM API into a backend service
- Build a full RAG pipeline from scratch — ingestion, retrieval, generation
- Work with vector databases and semantic search
- Ship AI-powered features in real products
- Debug and evaluate AI output systematically

**Previous:** [Layer 1 — Backend Foundations](layer1-backend.md)  
**Next:** [Layer 3 — Systems Thinking](layer3-systems.md)
