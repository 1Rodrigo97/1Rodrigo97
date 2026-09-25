<div align="right"><a href="README.md">Versão em português →</a></div>

# Rodrigo Martins

**Software Engineer | AI Engineering | Full Stack | RAG & Automation**

I build enterprise systems that integrate ERPs, BPM platforms, banking APIs, messaging APIs and language models — and that stay in production, used every day.

My work covers the whole cycle:

`business process → requirements → architecture → backend/frontend → API → database → integration → testing → troubleshooting → operation and evolution`

Getting the rules out of the person who owns the process is usually the hard part — and that is where the system is decided, not in the code.

---

## FlowMind AI

### RAG Engineering & Intelligent Automation Workbench

**→ [github.com/1Rodrigo97/flowmind-ai](https://github.com/1Rodrigo97/flowmind-ai)**

A workbench for Retrieval-Augmented Generation: document ingestion, vector retrieval, grounded answers with citations, and a lab to actually **measure** whether retrieval works — instead of assuming it does.

**Implemented**

- Ingestion of **PDF, DOCX, MD and TXT**, with **SHA-256** deduplication and chunking
- Local **embeddings** (`nomic-embed-text`, 768-d) and **vector search** on **pgvector**
- **Grounded generation** with source citations and an **explicit refusal when context is insufficient** — the system says it does not know instead of making something up
- **RAG Explorer** — retrieval inspection: the top-k retrieved chunks and their scores
- **RAG Evaluation Lab** — reproducible experiments measuring **Hit@K, MRR, Precision@K and Recall@K**, comparing baseline against experiment
- **BM25 lexical reranking** — behind a feature flag, off by default
- Index profiles that prevent embedding incompatibility
- **Pluggable** LLM and embedding providers
- **Automation with n8n** — document insights, retries, idempotency and observability

**Stack:** Python · FastAPI · SQLAlchemy 2 · PostgreSQL 16 + pgvector · Ollama (`llama3.2:3b`) · Vue 3 · TypeScript · Vite · Docker Compose · n8n

**Roadmap:** cross-encoder reranking · vLLM serving · dataset curation and fine-tuning · agents and tool calling

---

## Work on private systems

Beyond the public projects, I build private enterprise systems covering financial automation, HR, invoicing, integrations, APIs and Artificial Intelligence. **Code and data are not published, for confidentiality reasons.**

What those systems cover, in engineering terms:

| Domain | Nature of the work |
|---|---|
| Financial automation | Payment processing and tracking, banking integration over mTLS and OAuth2, idempotency and an audit trail |
| Enterprise integration | ERPs, BPM platforms and internal services, with authentication implemented by hand (OAuth 1.0a HMAC-SHA1, OAuth2, JWT, LDAP) |
| HR and recruiting | Job portal, LLM-based résumé parsing and screening, per-role fit scoring |
| Invoicing | Process automation and a support assistant on a messaging API, with output guardrails and handoff to a human |
| Accounting and tax | Daily reconciliation engines over the ERP, surfacing only what needs a human decision |
| Document validation | Document classification with a vision model, calibrated on real volume |
| Operational dashboards | Consolidated position and indicators for management |
| AI applied to process | Enterprise RAG, internal agents and event-driven automation |

---

## Stack

**Backend** — Python · FastAPI · Node.js · Express · REST APIs · SQLAlchemy · Sequelize · JWT · asynchronous processing

**Frontend** — Vue 3 · TypeScript · JavaScript · Vite · HTML · CSS · React · SPAs and admin dashboards

**Data** — PostgreSQL · Oracle · SQL · pgvector · MongoDB

**AI** — RAG · LLMs · SLMs · Ollama · embeddings · vector search · prompt engineering · grounded generation · RAG evaluation · BM25 reranking · TensorFlow · Keras · OpenCV · TFLite

**Automation and infrastructure** — n8n · Docker · Docker Compose · Git · GitHub · webhooks · event-driven pipelines · observability

---

## Currently studying

**vLLM** — model serving, OpenAI-compatible API, local inference, throughput, batching, concurrency, GPU and VRAM usage, and a practical comparison against Ollama. FlowMind was designed with a decoupled LLM provider precisely so this can land without rebuilding the RAG pipeline.

**Fine-tuning** — studying and preparing pipelines for dataset curation, training and evaluation. The target is behaviour, intent, classification and answer format — **not** mutable business rules, which change faster than a trained model can follow.

---

## Other public projects

**[Projeto-FullStack](https://github.com/1Rodrigo97/Projeto-FullStack)** — a monolithic Node.js + Express + Vue + PostgreSQL application: JWT authentication, protected CRUD, bulk CSV import (200k records), SQL-optimised pagination and an SPA consuming the API.

---

## Education

- **MSc in Applied Computing for Agronomy** — final stage
- **Postgraduate specialization** in Machine Learning
- **MBA** in Production Engineering
- **Postgraduate specialization** in Operations and Logistics Engineering
- **BEng in Mechatronics Engineering**

---

## Research

Experimental work, kept deliberately separate from the production systems described above.

**Machine learning and deep learning** — CNN · ResNet · MobileNet · YOLO
**Computer vision** — image classification · weed identification
**Edge AI** — TFLite and on-device inference
**Sensors and signals** — electronic nose · signal analysis · PCA · LDA · SVM

---

## Contact

**GitHub** · [1Rodrigo97](https://github.com/1Rodrigo97)
**LinkedIn** · [rodrigo-martins-198a32157](https://www.linkedin.com/in/rodrigo-martins-198a32157/)
**Email** · rodrigomartins246@gmail.com

---

<img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=1Rodrigo97&layout=compact&theme=tokyonight&hide_border=true" alt="Most used languages" height="150">
<img src="https://github-readme-stats-sigma-five.vercel.app/api?username=1Rodrigo97&show_icons=true&theme=tokyonight&hide_border=true&hide_title=true" alt="GitHub stats" height="150">
