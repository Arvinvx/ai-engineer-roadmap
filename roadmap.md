# Detailed Roadmap

Stage-by-stage breakdown with time estimates, topics, and what you should be able to do by the end of each one.

**Timeline note:** These estimates are for consistent part-time learners — around 1 to 3 hours a day. Full-time learners can compress them. Don't skip stages to save time. The foundation you build early determines how far you can go later.

## Stage 1 — Programming and Backend Foundations

**Time:** 2–4 months
**Resource:** [Scrimba Backend Developer Path](https://scrimba.com/the-backend-developer-path-c0tbi0l98f)

### JavaScript Fundamentals
- Variables, data types, functions, loops, conditionals
- Arrays and objects
- Async JavaScript — callbacks, promises, async/await
- ES6+ features
- Error handling

### Node.js and Server-Side Development
- What Node.js is and how the event loop works
- File system operations
- HTTP module
- npm and package management
- Environment variables with dotenv

### REST APIs
- What an API is and how HTTP works
- HTTP methods: GET, POST, PUT, PATCH, DELETE
- Status codes and response formats
- JSON as a data format
- Building REST APIs with Express.js
- Route params, query strings, request body
- API testing with Postman or Thunder Client

### Databases
- SQL — SELECT, INSERT, UPDATE, DELETE, JOIN
- Relational databases — PostgreSQL or SQLite
- MongoDB basics
- Database design — tables, relationships, primary/foreign keys
- Connecting a Node.js app to a database

### Authentication
- Sessions vs. JWT
- Password hashing with bcrypt
- Protecting routes with middleware
- Basic OAuth concepts

### Server Architecture
- MVC pattern
- Middleware chains in Express
- Error handling middleware
- Environment-based configuration

**End-of-stage goal:** A working REST API with user authentication, connected to a real database, with at least 5 routes. Deployed publicly on Railway, Render, or Fly.io.

## Stage 2 — Full-Stack Development

**Time:** 2–4 months
**Resources:** Scrimba continued + personal projects

### Frontend Basics
- HTML semantics
- CSS — Flexbox, Grid, responsive design
- Vanilla JS in the browser — DOM, events, fetch API
- Connecting a frontend to a backend API

### React
- Components and props
- State management with useState and useReducer
- Side effects with useEffect
- Fetching data from APIs
- React Router
- Forms and controlled components

### Full-Stack Architecture
- How frontend and backend communicate
- CORS
- Managing auth state in a single-page app
- Storing tokens (httpOnly cookies vs. localStorage tradeoffs)

### Deployment
- Frontend — Vercel, Netlify
- Backend — Railway, Render, Fly.io
- Databases — Supabase, PlanetScale, MongoDB Atlas
- Managing environment variables in production

**End-of-stage goal:** A full-stack app with user accounts, a real database, and a frontend. Doesn't need AI yet — it just needs to work.

## Stage 3 — Machine Learning Basics

**Time:** 1–2 months
**Resource:** [DeepLearning.AI Machine Learning Specialization](https://learn.deeplearning.ai/specializations/machine-learning)

### Supervised Learning
- What supervised learning is
- Regression and classification
- Training, validation, and test splits

### Core ML Concepts
- Cost functions
- Gradient descent
- Learning rate and hyperparameters
- Overfitting and underfitting
- Regularization — L1, L2
- Bias-variance tradeoff

### Neural Networks
- Layers, neurons, weights, biases
- Activation functions — ReLU, sigmoid, softmax
- Forward pass and backpropagation (conceptually)
- When neural networks make sense

### Practical ML
- Evaluating models — accuracy, precision, recall, F1
- Feature engineering basics
- scikit-learn for quick experiments

**End-of-stage goal:** Train a model on a real dataset. Understand why it makes the predictions it makes. Be able to evaluate whether it's actually performing well.

## Stage 4 — AI Engineering and LLM Apps

**Time:** 2–3 months
**Resource:** [Scrimba AI Engineer Path](https://scrimba.com/the-ai-engineer-path-c02v)

### Working with LLM APIs
- What an LLM is from an engineering perspective
- OpenAI API — completions, chat, function calling
- Anthropic API — messages, tool use
- Managing API keys securely
- Rate limiting, retries, and error handling
- Cost estimation and optimization

### Prompt Engineering
- System prompts vs. user messages
- Few-shot prompting
- Chain-of-thought prompting
- Prompt templates and variables
- Testing and iterating on prompts
- Avoiding prompt injection

### RAG — Retrieval-Augmented Generation
- What RAG is and why it exists
- Document chunking strategies
- Embeddings and what they represent
- Vector databases — Pinecone, Chroma, Weaviate
- Similarity search
- Building a full RAG pipeline end-to-end

### AI Agents
- What an AI agent is
- Tool use and function calling
- Memory — short-term (conversation history) vs. long-term (vector store)
- Multi-step reasoning patterns
- When agents make sense vs. simpler solutions

### Building AI Applications
- Streaming responses to the frontend
- Managing conversation state
- Adding AI features to existing apps
- Evaluating whether your AI feature is actually working

**End-of-stage goal:** Two complete AI apps — one using RAG, one using agents. Both deployed publicly.

## Stage 5 — LLM Internals

**Time:** 2–4 months
**Resources:**
- [Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter1/1)
- [Karpathy — Neural Networks: Zero to Hero](https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ)

### Transformers
- The attention mechanism
- Self-attention vs. cross-attention
- Multi-head attention
- Positional encoding
- Encoder-only, decoder-only, encoder-decoder architectures
- Why transformers replaced RNNs

### Tokenization
- What tokenization does and why it matters
- Byte Pair Encoding (BPE)
- How token count affects cost and context window
- Common tokenization gotchas

### Training
- Pre-training on large text corpora
- Next-token prediction as the training objective
- RLHF — Reinforcement Learning from Human Feedback

### Fine-Tuning
- When fine-tuning is appropriate vs. prompting or RAG
- Full fine-tuning vs. LoRA and QLoRA
- Preparing training data
- Using Hugging Face Transformers for fine-tuning

### Reading Research
- How to read an ML paper
- Key papers: Attention Is All You Need, GPT, BERT, LLaMA

**End-of-stage goal:** Implement a small language model from scratch following Karpathy's tutorials. Fine-tune a Hugging Face model on a custom dataset. Be able to explain how a transformer works out loud.

## Stage 6 — System Design

**Time:** Ongoing — come back to this continuously
**Resource:** [ByteByteGo System Design Playlist](https://www.youtube.com/watch?v=dGAgxozNWFE&list=PLCRMIe5FDPsd0gVs500xeOewfySTsmEjf&index=6)

### Scalability
- Vertical vs. horizontal scaling
- Stateless vs. stateful services
- Database replication and sharding
- CDN and static asset optimization

### Caching
- Cache invalidation strategies
- Redis — what it is and when to use it
- In-memory vs. distributed caching

### Queues and Async Processing
- Message queues and why they matter
- Kafka, RabbitMQ, and simpler queue options
- Worker processes and background jobs
- Handling long-running AI tasks asynchronously

### Load Balancing and High Availability
- How load balancers work
- Health checks and failover
- Rate limiting at the infrastructure level

### Databases at Scale
- SQL vs. NoSQL at scale
- Read replicas
- Connection pooling
- Indexing for query performance

### Designing AI Systems
- Architecting a RAG pipeline at scale
- Managing LLM latency in production
- Streaming and progressive rendering
- AI request queuing and prioritization
- Logging, tracing, and monitoring AI calls

**End-of-stage goal:** Be able to whiteboard a complete system design for an AI-powered product — from user request through the AI pipeline to the database and back.

## Timeline Summary

| Stage | Topic | Time |
|---|---|---|
| 1 | Programming and Backend | 2–4 months |
| 2 | Full-Stack Development | 2–4 months |
| 3 | Machine Learning Basics | 1–2 months |
| 4 | AI Engineering and LLM Apps | 2–3 months |
| 5 | LLM Internals | 2–4 months |
| 6 | System Design | Ongoing |
| **Total (part-time)** | | **11–17 months** |
| **Total (full-time)** | | **6–10 months** |

## How to Use This

Follow the stages in order. The sequence is intentional. Don't skip to Stage 4 because you want to "get to the AI part" — engineers who do that build fragile things and struggle when anything breaks.

Build something at the end of every stage. Learning without building doesn't stick.

Track your progress in [checklist.md](checklist.md).
