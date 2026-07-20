# 👋 Hi, I'm Naina Srivastava

**Backend & AI Systems Engineer** building real-time, voice-first applications and distributed systems that don't break. I specialize in low-latency AI inference, event-driven architectures, and complex data pipelines.

### ⚙️ Core Engineering Focus

*   **Real-Time AI Systems:** Voice interfaces, low-latency LLM inference (Groq), RAG pipelines, and agentic orchestration (LangChain).
*   **Distributed Systems:** Event-driven design, Transactional Outbox, Circuit Breakers, Idempotency, and stateless JWT security.
*   **High-Performance Backends:** FastAPI, asyncio, WebSockets, serverless deployment, and horizontal scaling.
*   **Data & State Management:** Redis for transient state and consensus, Qdrant for vector storage, PostgreSQL, and ETL pipelines.

### 🚀 Featured Projects

#### [ai_interviewer](https://github.com/naina-sriv/ai_interviewer)
A real-time, voice-conversational AI Interviewer that reads resumes, generates tailored questions using RAG from a company-specific database, and dynamically follows up on answers. Handles the full voice loop with browser-native STT/TTS and ultra-low-latency LLM inference via Groq.

**Key Challenges Solved:**
*   **Stateless Serverless:** Used Upstash Redis to persist session state across Vercel serverless functions.
*   **Voice UX:** Implemented silence detection (3-second debounce) and keep-alive mechanisms to prevent browser TTS/STT bugs.
*   **RAG Pipeline:** Integrated Qdrant vector DB with metadata filtering for company-specific question retrieval.
*   **Structured Output:** Enforced JSON schema constraints on the LLM for reliable parsing.

**Tech:** FastAPI, React, Redis, Groq (Llama 3.3), Qdrant, PyPDF2, Vercel

#### [catch-me-up](https://github.com/naina-sriv/catch-me-up)
A bot-free, enterprise-grade Meeting Copilot that captures live desktop audio from native apps (Discord, Zoom) and provides real-time transcriptions and AI summaries.

**Key Challenges Solved:**
*   **Universal Audio Capture:** Hooked into system audio using `chrome.desktopCapture` and Manifest V3 Offscreen Documents, bypassing service worker limitations.
*   **Backpressure Mitigation:** Used asyncio queues to handle 100ms binary streams without blocking the event loop.
*   **High-Throughput Deduplication:** Employed Redis Sorted Sets for transient consensus, inherently dropping duplicate uploads.
*   **Memory Optimization:** Designed "Eviction Cascades" to move older transcripts from Redis to Qdrant vector DB for long-term semantic retrieval.
*   **Stateless Security:** Implemented Discord-driven JWT RBAC, baking permissions into the token to avoid database lookups on every request.

**Tech:** FastAPI, WebSockets, Redis, Qdrant, Deepgram, LangChain, Gemini, Chrome Extension (Manifest V3)

#### [flash-sale-engine](https://github.com/naina-sriv/flash-sale-engine)
High‑concurrency flash sale system handling **10k+ RPS** with FastAPI async and Redis atomic operations. Features stateless JWT auth, rate-limiting, and Nginx horizontal scaling.

**Tech:** FastAPI, Redis, Docker, Nginx

#### [RouteIQ](https://github.com/naina-sriv/RouteIQ)
Route optimization engine solving **TSP and VRP** problems with Google OR-Tools and real road-network travel times from OSRM. Reduced repeated-request latency by **95%** with Redis caching.

**Tech:** OR-Tools, OSRM, Redis, Leaflet.js, Docker

#### [relay-dispatcher](https://github.com/naina-sriv/relay-dispatcher)
Standalone microservice for asynchronous workflows (emails, webhooks, Slack alerts) using the **Transactional Outbox pattern**. Implements horizontal worker scaling with Redis Streams and fault‑tolerant delivery.

**Tech:** Python, Redis, Transactional Outbox, Circuit Breakers

#### [parivartan-legal](https://github.com/naina-sriv/parivartan-legal)
End-to-end ETL pipeline for legal documents: PDF → text extraction → AI summarization with Gemini API (Groq fallback). Deployed on AWS EC2 with GitHub Actions CI/CD.

**Tech:** Python, PostgreSQL, SQLAlchemy, gRPC, AWS, Gemini API

#### [ftp (Fixing The Platform)](https://github.com/naina-sriv/ftp)
Constituency-bound civic issue reporting platform with **community threshold-based escalation**. Ensures zero cross-constituency noise with JWT-based scoped authentication.

**Tech:** FastAPI, PostgreSQL, Celery, Redis, JWT

#### [profilr-backend](https://github.com/naina-sriv/profilr-backend)
Data pipeline and analysis tool that ingests CSV files to generate structured JSON reports with missing value analysis, outlier detection (IQR), and correlation matrices.

**Tech:** FastAPI, Streamlit, Pandas

---

### 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-EE4C2C?style=flat-square&logo=qdrant&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-0040A1?style=flat-square&logo=groq&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3F?style=flat-square&logo=amazon-aws&logoColor=white)

---

### 💬 "If you can't explain it simply, you haven't built it resiliently yet."

### 📫 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/naina-srivastava)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white)](https://twitter.com/naina_sriv)
