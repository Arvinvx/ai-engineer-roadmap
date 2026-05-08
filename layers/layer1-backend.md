# Layer 1 — Backend Foundations

**Course:** [Scrimba Backend Developer Path](https://scrimba.com/the-backend-developer-path-c0tbi0l98f)  
**Timeline:** May 2026 – Jul 2026  
**Goal:** Build the server-side foundation that every AI product runs on top of.

---

## What You Learn

### 1. Node.js Core

Before frameworks, you need to understand the runtime itself.

- How Node.js works: event loop, non-blocking I/O, the V8 engine
- Modules: CommonJS (`require`) vs ES Modules (`import`)
- Built-in modules: `fs`, `path`, `http`, `os`, `events`
- Asynchronous patterns: callbacks → Promises → async/await
- Error handling in async code
- Streams and buffers — reading/writing large data efficiently

**Why it matters:** Node's async model is what makes it fast enough to serve thousands of concurrent API requests — the same model underpins most AI backend infrastructure.

---

### 2. Express.js — Building APIs

The most widely used Node.js framework. Minimal, fast, and unopinionated.

- Setting up an Express server from scratch
- Routing: `GET`, `POST`, `PUT`, `DELETE`
- Route parameters and query strings
- Middleware: what it is, how the stack works, writing your own
- Built-in middleware: `express.json()`, `express.static()`
- Third-party middleware: `cors`, `morgan`, `helmet`
- Error-handling middleware — the 4-argument pattern
- Structuring a real project: routes, controllers, services

**Why it matters:** Every AI API you build — whether it's a RAG endpoint, an inference proxy, or a webhook handler — is an Express app.

---

### 3. MongoDB & Mongoose

Document databases are the most common choice for AI product backends.

- What NoSQL means and when to use it over SQL
- MongoDB data model: documents, collections, BSON
- CRUD operations: `insertOne`, `find`, `updateOne`, `deleteOne`
- Querying: filters, projections, sorting, pagination
- Mongoose: schemas, models, validation
- Relationships in MongoDB: embedding vs referencing
- Indexing for query performance
- Aggregation pipeline basics

**Why it matters:** Storing user sessions, conversation history, embeddings metadata, and API logs all go through a database. Knowing how to model and query that data efficiently is non-negotiable.

---

### 4. Authentication & Security

Every real product needs auth. Most security vulnerabilities live here.

- Sessions vs tokens — when to use each
- JWT (JSON Web Tokens): structure, signing, verification, expiry
- `bcrypt` for password hashing — never store plaintext
- HTTP-only cookies vs localStorage — the security tradeoff
- OAuth 2.0 flow: authorizing with Google, GitHub
- Role-based access control (RBAC)
- Rate limiting with `express-rate-limit`
- Helmet.js — setting secure HTTP headers
- Input validation and sanitization to prevent injection

**Why it matters:** AI products handle sensitive data. A leaked API key or exposed user data kills trust and can kill the product. Auth done right from the start saves enormous pain later.

---

### 5. REST API Design

APIs are interfaces. Good design makes them easy to use and maintain.

- REST principles: statelessness, uniform interface, resources
- URL design: naming conventions, nesting, versioning (`/v1/`)
- HTTP status codes — using the right ones (`200`, `201`, `400`, `401`, `403`, `404`, `500`)
- Request/response structure: consistent JSON envelopes
- Pagination patterns: offset vs cursor-based
- API documentation with tools like Swagger/OpenAPI
- Handling errors gracefully with structured error responses

**Why it matters:** You'll consume and build APIs constantly. A well-designed API is self-documenting and predictable. A poorly designed one creates bugs at every integration point.

---

### 6. Environment, Config & Deployment Basics

How real apps manage configuration and get shipped.

- `.env` files and `dotenv` — never hardcode secrets
- Environment-specific config: development, staging, production
- `nodemon` for development auto-reload
- Process management with PM2 in production
- Basic deployment: VPS (DigitalOcean, Railway, Render)
- Environment variables in deployment platforms
- Logging best practices — structured logs with `winston` or `pino`

**Why it matters:** A backend that only runs on your laptop isn't a backend. Understanding deployment from the start means you can ship things end-to-end, not just build locally.

---

## Skills Unlocked After This Layer

By the end of Layer 1, you can:

- Build a production-ready REST API from scratch
- Handle authentication, sessions, and user data securely
- Model and query a MongoDB database
- Deploy a Node.js backend to a live server
- Structure a real codebase that scales beyond a single file

**Next:** [Layer 2 — AI Engineering Core](layer2-ai-engineering.md)
