# Portfolio Projects

Building real things is how you actually learn, and it's the most important thing you can show employers. This is a list of project ideas across three levels.

A few things before you start:

Build things you would actually use or that solve a real problem. Document your decisions — why did you build it this way, what would you do differently. Ship it publicly. A deployed project with one feature beats a local project with ten.

## Beginner Projects

Good after completing Stages 1–2 and starting Stage 4.

### 1. AI Chatbot with Conversation Memory

A chat interface that remembers what you said earlier and responds coherently to follow-up questions. Sounds simple but there's a lot to learn in the implementation.

What you'll learn: LLM API integration, managing conversation history, streaming responses to a UI.

Tech: Node.js or Python, OpenAI or Anthropic API, React or vanilla JS

Extensions: Add different personas users can switch between. Store conversation history in a database so users can come back to old chats. Add a system prompt editor.

### 2. RAG Document Assistant

Upload a PDF or paste in text, then ask questions about it. The AI answers based only on that document — no hallucinating information that isn't there.

What you'll learn: Document chunking, generating and storing embeddings, vector similarity search, building a full RAG pipeline.

Tech: Node.js or Python, OpenAI embeddings, Chroma or Pinecone, Express or FastAPI

Extensions: Support multiple documents. Show the exact source passages used to answer. Add a fallback when the answer isn't in the document.

### 3. AI Note Summarizer

Paste in meeting notes or a long article and get a structured summary — key points, action items, decisions made.

What you'll learn: Structured output prompting, working with long inputs, prompt templates.

Extensions: Integrate with Notion or Google Docs. Auto-detect the note type and adjust the summary format. Generate follow-up questions.

### 4. AI Flashcard Generator

Paste in study material and get a set of flashcards as question-answer pairs.

What you'll learn: Structured JSON output from LLMs, content parsing, simple data persistence.

Extensions: Build spaced repetition. Let users rate cards and track retention. Export to Anki format.

### 5. Semantic Search App

A search interface where results are ranked by meaning, not keyword matching. Search a collection of articles, books, or product descriptions and find relevant results even when the exact words don't match.

What you'll learn: Embeddings, vector search, the practical difference between lexical and semantic search.

Extensions: Compare semantic vs. keyword search results side by side. Build over a public dataset.

## Intermediate Projects

Good after finishing Stage 4 with at least one beginner project shipped.

### 6. AI Customer Support Agent

A chatbot that handles customer support for a hypothetical business. Answers questions from a knowledge base, escalates when it can't help, and logs all conversations.

What you'll learn: RAG with a knowledge base, escalation logic, conversation state management, logging AI interactions.

Tech: Node.js or Python, LLM API, vector database, SQL for logs

Extensions: Build an admin dashboard to review conversations. Track common questions. Add email escalation via a simple SMTP integration.

### 7. AI Booking Assistant for Local Businesses

A chat interface for a barbershop, salon, or restaurant that helps customers check availability and book appointments using natural language.

What you'll learn: Function calling / tool use, integrating AI with real data (a calendar or booking system), handling ambiguous user intent.

Tech: Node.js or Python, LLM API with tool use, calendar API or mock booking system

Extensions: Google Calendar integration. SMS confirmation via Twilio. Multiple language support.

### 8. AI Study Assistant

An AI that helps students learn a topic. It explains concepts, quizzes the user, answers follow-up questions, and tracks what the user has and hasn't understood yet.

What you'll learn: Multi-turn conversation design, adaptive behavior based on user performance, combining RAG with conversation management.

Extensions: Upload a syllabus and generate a study plan. Auto-graded practice exams with explanations.

### 9. AI Code Review Assistant

Paste or upload code and get a review — bugs, security issues, performance problems, style.

What you'll learn: Prompting for structured technical output, handling code as input safely, building useful developer tools.

Extensions: GitHub Action that runs on every PR. Support for custom coding standards.

### 10. Multi-Source Research Tool

Enter a research question, the app searches multiple sources (web search, uploaded documents, a knowledge base), synthesizes results, and returns a well-cited answer.

What you'll learn: Multi-source RAG, web search API integration, source citation in AI responses.

Tech: Python or Node.js, LLM API, web search API (Tavily, SerpAPI), vector database

Extensions: Export research as a formatted report. Let users filter which sources to include.

## Advanced Projects

Good after finishing Stages 5–6 with multiple intermediate projects shipped.

### 11. Full-Stack SaaS with AI Features

A complete product with paying users, AI as a core feature, user accounts, billing, and real production infrastructure.

What you'll learn: Subscription billing with Stripe, production architecture, AI cost management, operational concerns like monitoring and rate limiting.

Ideas: AI writing assistant for a specific niche. AI data analysis tool for small businesses. AI-powered CRM feature.

### 12. AI Lead Generation and Outreach Tool

Takes a target customer profile, finds relevant companies or people, researches them, and drafts personalized outreach messages.

What you'll learn: Multi-step AI pipelines, integrating external data APIs, handling large volumes of requests, building AI systems with human review steps.

Extensions: CRM integration. Track response rates and feed that back into the prompts.

### 13. Fine-Tuned Domain-Specific Model

Fine-tune an open-source LLM on a specific domain — customer support transcripts, legal documents, a specific writing style.

What you'll learn: Preparing training data, fine-tuning with Hugging Face LoRA/QLoRA, evaluating a fine-tuned model vs. a base model, deploying a custom model.

Tech: Python, Hugging Face Transformers, GPU (Google Colab or RunPod)

### 14. Real-Time AI Data Pipeline

Ingests a real-time data stream — social media, news, support tickets — processes each item with an AI model, and routes results based on classification.

What you'll learn: Streaming data architecture, AI classification at scale, message queues, designing for throughput and cost.

### 15. Multi-Agent System

Multiple AI agents collaborating on a complex task — a research agent, writing agent, fact-checking agent, and editing agent working together to produce a finished output.

What you'll learn: Agent orchestration patterns, designing handoffs between agents, handling failure in multi-step pipelines, evaluating agent performance.

## Tips That Apply to All of These

Start with the user, not the technology. What problem does this solve? For who? What does success actually look like?

Define what "good" means before you build. What makes a good AI response for your use case? Build a small eval set and test your prompts against it systematically.

Write about what you built. A short LinkedIn post or blog entry explaining why you built it, what you learned, and what you'd do differently next time doubles the value of every project. It also starts building your public presence before you need it.
