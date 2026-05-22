# Nit Patel

**ML Engineering · Model Training & Evaluation · Inference Optimization**

BTech IT · BVM Engineering College · CGPA 8.78 · Graduating 2026  
AI Engineer @ AppMixo Solution, Surat

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/nit-patel-ba61441a3)
[![PyPI](https://img.shields.io/badge/PyPI-rag--reranker-3775A9?style=flat&logo=pypi&logoColor=white)](https://pypi.org/project/rag-reranker/)
[![Email](https://img.shields.io/badge/Email-Nehnit23%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:Nehnit23@gmail.com)

---

## What I'm trying to do

Most of my work so far has been building *with* models — RAG pipelines, multi-agent systems, LLM-backed APIs. I'm now focused on understanding and improving the models themselves.

I implemented a decoder-only transformer from scratch in PyTorch — every component written manually, no HuggingFace trainer, trained on 10M tokens with loss-curve validation. Not because I needed to, but because I wanted to understand what attention heads are actually computing before trusting them in production. That's the level I try to operate at.

Currently studying: training dynamics, LoRA/QLoRA and fine-tuning math (SFT, RLHF, DPO), KV cache bottlenecks, quantization (INT4/INT8/GPTQ), and behavioural evaluation design.

---

## Selected Projects

### 🧠 [Decoder-Only GPT — Trained from Scratch](https://github.com/Nit2312)
Implemented a full decoder-only transformer from first principles in PyTorch:
multi-head self-attention, causal masking, positional embeddings, layer norm,
residual connections, weight tying. Wrote the training loop manually — gradient
accumulation, checkpoint logic, LR scheduling. Trained on 10M tokens on CUDA
and tracked the loss curve throughout to verify coherent next-token learning.

> Built to understand internals, not just call an API.

`PyTorch` `CUDA` `NumPy`

---

### 📦 [rag-reranker](https://pypi.org/project/rag-reranker/) — Published on PyPI
Cross-encoder reranking library using `ms-marco-MiniLM-L-6-v2`. Scores full
query–document pairs rather than relying on embedding similarity alone, improving
retrieval precision as a post-retrieval stage in any RAG pipeline.
Includes evaluation tooling to measure NDCG and MRR improvement over
bi-encoder-only baselines.

`sentence-transformers` `cross-encoder` `PyPI`

---

### 🏭 Anti-Hallucination Order Risk System — AppMixo *(Production, 2026)*
Deterministic risk engine for a B2B POS platform where financial decisions are
at stake. Architecture principle: every decision flag is pre-computed before the LLM
is invoked — the model explains decisions, never makes them. Includes early-exit
filters that cut unnecessary inference calls (10× token reduction), a confidence
gate on the Vision pipeline that rejects low-quality inputs rather than hallucinating,
and a LangChain tool-routing agent for pricing intelligence.

**~40% reduction in manual cart-entry errors in production. 1st Place, BVM Project Expo 2026 (60+ teams).**

> Private repo — documentation available on request.

`LangChain` `OpenAI API` `MongoDB` `Docker`

---

### 📊 [Multi-Asset RAG System](https://github.com/Nit2312/Multi_AI_agent)
Financial advisory RAG with asset-based vector store routing, cross-encoder
reranking (top-50 → rerank → top-10 to LLM), and RAGAS evaluation for
continuous retrieval quality monitoring.

`LangChain` `LangGraph` `AstraDB` `RAGAS` `Groq`

---

### 🤖 [Multi-Agent Research Pipeline](https://github.com/Nit2312/Multi_AI_agent)
Hierarchical multi-agent system (researcher → writer → evaluator → supervisor)
built in LangGraph with episodic, procedural, and semantic memory. Agent-to-agent
handoffs with pre/post-model guardrails exposed via FastAPI.

`LangGraph` `LangSmith` `FastAPI` `Python`

---

### 🛒 [Flipkart Product Recommender](https://github.com/Nit2312/flipkart_product_recommender)
RAG-based recommendation engine deployed on GCP with Docker and Kubernetes.
Prometheus + Grafana for real-time pipeline monitoring.

`GCP` `Docker` `Kubernetes` `Prometheus` `Grafana`

---

## Stack

```
ML & Training      PyTorch · CUDA · Transformers (from scratch) · LoRA/QLoRA (study)
                   SFT / RLHF / DPO (study) · Loss-curve analysis

Evaluation         RAGAS · Held-out eval design · Behavioural testing
                   Cross-encoder scoring · NDCG / MRR

LLM Frameworks     LangChain · LangGraph · LangSmith · OpenAI API
                   Hugging Face · OpenRouter

Retrieval & RAG    RAG pipeline design · Vector search · Cross-encoder reranking
                   AstraDB · Chroma · Hybrid retrieval

Infra              Docker · Kubernetes · GCP · AWS · Prometheus · Grafana

Backend            FastAPI · Flask · Python · SQL

Databases          PostgreSQL · MongoDB · Redis · Firebase
```

---

## What I'm thinking about

The gap between a RAG demo and a system that holds up in production six months later is almost entirely about evaluation, monitoring, and failure-mode design — not model choice. The same principle applies one level down: the gap between a fine-tuned model and a reliable one is about understanding the training dynamics, not just running the script.

Currently reading: *Designing Data-Intensive Applications* (Kleppmann) · *Mathematics for Machine Learning* (Deisenroth) · Attention Is All You Need and its follow-up literature.

---

## Experience

| Role | Company | Period |
|---|---|---|
| AI Engineer (Full-Time) | AppMixo Solution, Surat | May 2026 – Present |
| AI/ML Intern | AppMixo Solution, Surat | Dec 2025 – Apr 2026 |
| Gen AI Intern | Akhiyam Solutions (Remote) | Oct 2025 – Dec 2025 |
| AI/ML Intern | EdgeQomputing LLP, Surat | Jun 2025 – Jul 2025 |

---

📧 Nehnit23@gmail.com · [LinkedIn](https://linkedin.com/in/nit-patel-ba61441a3) · Surat, Gujarat, India
