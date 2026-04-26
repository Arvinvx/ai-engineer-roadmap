# AI Engineer Roadmap

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

A practical roadmap for people who want to become AI engineers by learning backend development, full-stack development, machine learning basics, LLMs, AI apps, and system design.

No hype. No "become an AI engineer in 30 days." Just a realistic path with real resources and real projects.

## Who This Is For

| Audience | Why this works for you |
|---|---|
| Complete beginners | Starts from scratch, no assumed knowledge |
| Self-taught developers | Fills the gaps in backend, ML, and AI systematically |
| Web developers moving into AI | Builds on what you already know |
| CS students | Practical and project-focused, good supplement to theory |
| People building AI products | Teaches the full stack you need to actually ship things |

## The Roadmap

```
Stage 1 → Programming & Backend Foundations     (2–4 months)
Stage 2 → Full-Stack Development                (2–4 months)
Stage 3 → Machine Learning Basics               (1–2 months)
Stage 4 → AI Engineering & LLM Apps            (2–3 months)
Stage 5 → LLM Internals                         (2–4 months)
Stage 6 → System Design                         (ongoing)
Stage 7 → Portfolio Projects
Stage 8 → Career Direction
```

See [roadmap.md](roadmap.md) for the full breakdown with time estimates and topic lists.

## Stage 1 — Programming and Backend Foundations

**Resource:** [Scrimba Backend Developer Path](https://scrimba.com/the-backend-developer-path-c0tbi0l98f)
*(General Scrimba link: [scrimba.com](https://scrimba.com/?via=u43d5376) — heads up, this is a referral link)*

Before you touch AI, you need to understand how software is actually built. AI engineers write server-side code, call APIs, manage databases, and deploy applications. This stage gets you there.

**Topics:**
- Node.js and JavaScript for backend
- REST APIs and HTTP
- Databases — SQL and NoSQL
- Authentication and authorization
- Server architecture and routing
- Real backend projects

AI models are tools. To use them well, you need to already know how to build the systems around them.

## Stage 2 — Full-Stack Development

**Resource:** [Scrimba Backend Developer Path](https://scrimba.com/the-backend-developer-path-c0tbi0l98f) (continued) + your own projects

Most AI-powered products are full-stack apps with AI built in. If you only know the AI part and nothing about how real apps work, you're going to hit walls constantly.

**Topics:**
- Frontend basics (HTML, CSS, JavaScript)
- Connecting a frontend to a backend API
- Databases and data modeling
- Auth flows — sessions, JWT, OAuth
- Deployment and environment config
- Building and shipping full projects end-to-end

## Stage 3 — Machine Learning Basics

**Resource:** [DeepLearning.AI Machine Learning Specialization](https://learn.deeplearning.ai/specializations/machine-learning)

You don't need to be a math PhD to be an AI engineer. But you do need to understand how models actually learn — not just how to call an API. This stage gives you that foundation.

**Topics:**
- Supervised learning — regression and classification
- Cost functions and gradient descent
- Overfitting, regularization, and model evaluation
- Basic neural networks
- Decision trees and ensemble methods
- Practical ML intuition — when to use what

When something breaks in an AI feature, the engineers who understand how models work are the ones who can actually fix it.

## Stage 4 — AI Engineering and LLM Apps

**Resource:** [Scrimba AI Engineer Path](https://scrimba.com/the-ai-engineer-path-c02v)
*(General Scrimba link: [scrimba.com](https://scrimba.com/?via=u43d5376) — referral link)*

This is the core of what AI engineers actually do day-to-day. Building real apps with LLMs, shipping AI features, and making them work reliably in production.

**Topics:**
- Using LLM APIs (OpenAI, Anthropic, etc.)
- Prompt engineering that works at scale
- Retrieval-Augmented Generation (RAG)
- Embeddings and semantic search
- Vector databases — Pinecone, Weaviate, Chroma
- AI agents and tool use
- Building AI-powered apps end-to-end
- Adding AI features to existing products

## Stage 5 — LLM Internals

**Resources:**
- [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1)
- [Andrej Karpathy — Neural Networks: Zero to Hero](https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ)

Going under the hood makes you a significantly better AI engineer. You'll make better decisions, debug problems faster, and understand why things work the way they do.

**Topics:**
- Transformers and the attention mechanism
- Tokenization and embedding spaces
- How neural networks learn
- Training and fine-tuning basics
- When to fine-tune vs. prompt engineer vs. RAG
- Reading model cards and research papers

## Stage 6 — System Design

**Resource:** [ByteByteGo System Design Playlist](https://www.youtube.com/watch?v=dGAgxozNWFE&list=PLCRMIe5FDPsd0gVs500xeOewfySTsmEjf&index=6)

AI systems at scale have the same challenges as any distributed system — plus a few new ones. This is what separates engineers who can build demos from engineers who can build products.

**Topics:**
- Scalability patterns
- Caching — Redis, CDN
- Message queues — Kafka, RabbitMQ
- Load balancing
- Database design at scale
- Distributed systems
- Designing real production AI pipelines

## Stage 7 — Portfolio Projects

See [projects.md](projects.md) for the full list with descriptions.

| Level | Project |
|---|---|
| Beginner | AI chatbot with conversation memory |
| Beginner | RAG document assistant — ask questions about a PDF |
| Intermediate | AI customer support agent with escalation |
| Intermediate | AI booking assistant for local businesses |
| Intermediate | AI study assistant — summarize, quiz, explain |
| Advanced | Full-stack SaaS with AI features |
| Advanced | AI lead generation tool |
| Advanced | Multi-agent system with tool use |

Build things you would actually use or that solve a real problem. Generic chatbots are everywhere. Projects with a specific use case or niche are what stand out.

## Stage 8 — Career Direction

AI engineering job titles are still evolving. Here's what the common ones actually mean:

| Title | Focus |
|---|---|
| AI Engineer | Building apps and features using LLMs |
| Full-Stack AI Engineer | End-to-end product development with AI |
| LLM Engineer | Deep specialization in large language models |
| AI Product Engineer | AI engineering with a product and user focus |
| Backend AI Engineer | Server-side infrastructure for AI systems |
| ML Engineer | Training, fine-tuning, and deploying models |

Most entry-level AI engineering roles are closer to "software engineer who works with AI APIs" than "ML researcher." Get the software fundamentals solid first.

## Files in This Repo

| File | What's inside |
|---|---|
| [README.md](README.md) | This overview |
| [roadmap.md](roadmap.md) | Detailed stage breakdown with time estimates |
| [resources.md](resources.md) | All resources with links and notes |
| [projects.md](projects.md) | Project ideas from beginner to advanced |
| [checklist.md](checklist.md) | Checkbox progress tracker |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute |
| [LICENSE](LICENSE) | MIT |

## Contributing

Open source project — if you find a better resource, want to add a project idea, or spot something outdated, PRs and issues are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE) — free to use, share, and modify with attribution.

*Not sponsored by any platform listed. The Scrimba referral link is an affiliate link — it's included because the courses are actually good, not because of the commission.*
