# Nit Patel — AI Engineer

I build production AI systems where the architecture decisions matter as much as the model choice.

Currently finishing BTech in Information Technology at BVM Engineering (2026, CGPA 8.78) while working as AI Systems Architect at AppMixo Solution, Surat.

---

## What I Actually Build

Most AI engineers bolt an LLM onto an existing system and call it done. I design the layer between the business logic and the model — the part that determines whether the system is reliable in production or just impressive in demos.

At AppMixo I architected an order risk system for a production POS backend where hallucination is not acceptable — financial decisions were at stake. The solution: a deterministic facts engine that pre-computes every decision flag before the LLM is invoked. The model explains decisions. It never makes them. That system is live and handling real orders.

That's the kind of problem I find interesting.

---

## Core Stack

```
AI/ML          LangChain · LangGraph · LangSmith · Hugging Face · OpenAI API
               RAG Pipelines · Multi-Agent Systems · Prompt Engineering · RAGAS
               
Infra          Docker · Kubernetes · GCP · AWS · CI/CD
               Prometheus · Grafana · AstraDB · MongoDB · PostgreSQL · Redis

Languages      Python · JavaScript · SQL · Java · C++
```

---

## Selected Projects

### Anti-Hallucination Order Risk System — AppMixo *(Production, 2026)*
Rule-based scoring engine + LangChain tool-routing agent for POS order decisioning. LLM constrained to pre-computed explicit facts only — zero hallucination on financial decisions. Includes early-exit filters, fraud detection integration, and multi-address behavioural analysis.
> Private repo — documentation available on request

---

### [Multi-Asset RAG System](https://github.com/Nit2312/Multi_AI_agent)
Financial advisory RAG with asset-based vector store routing, cross-encoder reranking (top-50 → rerank → top-10 to LLM), and automated RAGAS evaluation for continuous quality monitoring. Built with LangChain, AstraDB, LangGraph, Groq.

---

### [GPT Language Model — Trained from Scratch](https://github.com/Nit2312)
Decoder-only transformer implemented from first principles — multi-head self-attention, positional embeddings, custom BPE tokenizer, AdamW optimisation. Trained on 10M tokens on CUDA. Built to understand what's happening underneath the frameworks.

---

### [Flipkart Product Recommender](https://github.com/Nit2312/flipkart_product_recommender)
RAG-based recommendation engine deployed on GCP with Docker and Kubernetes. Prometheus + Grafana for real-time pipeline monitoring. Part of an LLMOps series focused on production deployment patterns.

---

### [Multi-Agent AI System — Akhiyam](https://github.com/Nit2312/Multi_AI_agent)
Hierarchical multi-agent system with LangGraph — researcher, writer, evaluator, and supervisor agents with episodic, procedural, and semantic memory. Agent-to-agent handoffs with pre/post-model guardrails via FastAPI.

---

## Experience

**AI/ML Intern — AI Systems Lead** | AppMixo Solution, Surat | Dec 2025 – Apr 2026
Sole AI architect on a production POS platform. Designed anti-hallucination order risk system, product intelligence module, cart vision pipeline, and AI dashboard. Led implementation team.

**Gen AI Intern** | Akhiyam Solutions, Remote | Oct 2025 – Dec 2025
Built hierarchical multi-agent systems with LangGraph. FastAPI backends with agent orchestration and guardrails.

**AI/ML Intern** | EdgeQomputing LLP, Surat | Jun 2025 – Jul 2025
Production RAG pipeline for patent review using LangChain, Hugging Face embeddings, Groq-hosted LLaMA 3.

---

## What I'm Thinking About

The gap between a RAG demo and a RAG system that works in production six months later is almost entirely about evaluation, monitoring, and data quality — not model choice. I'm currently focused on RAGAS-based continuous evaluation pipelines and corrective retrieval architectures (CRAG) for production systems.

I trained a GPT from scratch not because I needed to, but because I wanted to understand what attention heads are actually computing before I trusted them in production. That's the level I try to operate at.

---

## Let's Talk

If you're working on production AI systems, RAG infrastructure, or agentic architectures — I'm interested.

📧 Nehnit23@gmail.com
💼 [LinkedIn](https://www.linkedin.com/in/nit-patel-ba61441a3/)
📍 Surat, Gujarat
