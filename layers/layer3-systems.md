# Layer 3 — Systems Thinking

**Course:** [ByteByteGo — GenAI System Design](https://bytebytego.com/courses/genai-system-design-interview) · [YouTube Channel](https://www.youtube.com/@ByteByteGo)  
**Timeline:** Nov 2026 – Jan 2027  
**Goal:** Design AI systems that scale reliably under real-world load.

---

## What You Learn

### 1. Distributed Systems Fundamentals

The mental model behind every large-scale system.

- Vertical vs horizontal scaling — when each breaks down
- CAP theorem: consistency, availability, partition tolerance
- ACID vs BASE — database guarantees and tradeoffs
- Synchronous vs asynchronous communication
- Idempotency — designing operations that are safe to retry
- Consensus and coordination: how distributed nodes agree
- Failure modes: network partitions, split-brain, cascade failures

**Why it matters:** AI systems at scale are distributed systems. If you don't understand these fundamentals, you'll build systems that fail in unexpected ways under load.

---

### 2. Load Balancing & API Gateways

How traffic gets routed across a system.

- Round-robin, least connections, and weighted routing strategies
- Sticky sessions — when you need a user to hit the same server
- Health checks and automatic failover
- API gateways: rate limiting, auth, routing, request transformation
- Reverse proxies: Nginx, Caddy
- Layer 4 vs Layer 7 load balancing

**Why it matters:** An AI API that works for 10 users and falls over at 1,000 isn't a product. Load balancing is how you make sure inference requests, RAG queries, and chat sessions stay fast as volume grows.

---

### 3. Caching Strategies

The most powerful tool for reducing latency and cost.

- Cache-aside, write-through, write-back patterns
- Redis fundamentals: data structures, TTL, eviction policies
- CDN caching for static assets and edge responses
- Semantic caching: caching LLM responses by meaning, not exact string
- Cache invalidation — why it's hard and how to do it right
- What not to cache: when freshness matters more than speed

**Why it matters:** LLM inference is expensive. Caching semantically similar queries can reduce API costs by 40-70% in production. This is a direct cost lever for any AI product.

---

### 4. Message Queues & Async Processing

Decoupling producers and consumers for resilient systems.

- Why queues: smoothing traffic spikes, retry logic, backpressure
- Message queue concepts: producers, consumers, acknowledgements, dead-letter queues
- Tools: Redis Pub/Sub, BullMQ, RabbitMQ, Kafka (at scale)
- Job queues for AI: batching inference requests, async document processing
- Exactly-once vs at-least-once delivery — the tradeoff
- Monitoring queue depth and processing lag

**Why it matters:** Document ingestion, batch embeddings, async report generation — these are all queue jobs. Async processing is what makes AI backends feel responsive even when the underlying work takes seconds.

---

### 5. Database Scaling

What to do when a single database isn't enough.

- Read replicas: offloading read traffic
- Database sharding: partitioning data across instances
- Connection pooling — why raw connections don't scale
- Indexing strategy: composite indexes, partial indexes, covering indexes
- N+1 query problem and how to fix it
- When to use SQL vs NoSQL vs vector databases
- pgvector: storing and querying embeddings inside PostgreSQL

**Why it matters:** Your AI product's knowledge base, user data, and conversation history all live in databases. Understanding how to keep queries fast as data grows is what separates prototypes from products.

---

### 6. GenAI System Design Patterns

ByteByteGo's specialized curriculum on designing AI-specific systems.

- LLM serving infrastructure: model hosting, batching, GPU allocation
- RAG at scale: sharded vector indexes, multi-tenant retrieval
- Streaming architectures for real-time AI responses
- Model versioning and A/B testing in production
- Designing for LLM latency: p50/p95/p99 and what affects each
- Prompt caching: how providers cache KV state across requests
- Multi-agent system design: orchestration, communication, failure handling
- Cost modeling: estimating and controlling inference spend

**Why it matters:** These are the patterns behind ChatGPT, Perplexity, and every serious AI product. Understanding them lets you design systems that hold up in production — not just in demos.

---

### 7. Observability & Monitoring

You can't improve what you can't measure.

- The three pillars: logs, metrics, traces
- Structured logging — making logs queryable
- Distributed tracing across services: OpenTelemetry
- Key AI-specific metrics: latency per token, cache hit rate, hallucination rate
- Alerting: what to page on vs what to track passively
- LLM observability tools: LangSmith, Helicone, Langfuse
- Cost dashboards: tracking token usage by feature and user

**Why it matters:** In production, things break in ways you didn't predict. Observability is how you find out fast, diagnose the cause, and fix it before users churn.

---

## Skills Unlocked After This Layer

By the end of Layer 3, you can:

- Design a scalable AI system architecture from scratch
- Identify bottlenecks and choose the right scaling strategy
- Implement caching, queuing, and async processing in an AI backend
- Reason about cost and latency tradeoffs in system design interviews
- Monitor and debug distributed AI systems in production

**Previous:** [Layer 2 — AI Engineering Core](layer2-ai-engineering.md)  
**Next:** [Layer 4 — Deep ML Understanding](layer4-deep-ml.md)
