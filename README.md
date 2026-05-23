# Sarala Biswal

**VP / Director of AI Engineering · AI Platform Architect · Agentic AI · MCP · MLOps · Enterprise Scale · Oracle CPQ · Quote-to-Cash**

*Belmont, CA · He/Him*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-saralabiswal-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal)
[![Email](https://img.shields.io/badge/Email-saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)
[![Profile Views](https://komarev.com/ghpvc/?username=saralabiswal&style=flat-square&color=3b82f6&label=Profile+Views)](https://github.com/saralabiswal)

---

## About

I build AI/ML platforms that generate revenue — not just predictions.
Hands-on engineering leader who architects production systems personally while setting technical direction for a 40+ person global org.

17+ years at Oracle shipping two flagship AI platforms at enterprise scale:

- **Agentic AI on CPQ** — Renewal Agent + Quote Generation Agent · 300,000+ sales users · 600+ enterprise clients · 50+ countries · 30% renewal cycle compression · 28% quote processing efficiency improvement
- **Unity CDP AI/ML** — 6 production models (Next Best Action, Churn Propensity, CLV, RFM Segmentation, Multi-Touch Attribution, MMM) · 9,000+ customers at day-one GA · no phased rollout

The hard part isn't the model — it's the integration layer. I solved the cross-vendor problem in production: unified live context from Salesforce, MS Dynamics, and Oracle clouds so agents make decisions on real data, not cached snapshots.

---

## Featured Projects

### 🏦 [Banking Agentic AI Platform](https://github.com/saralabiswal/agentic-banking-llmops)

> A cloud-agnostic, production-grade Agentic AI platform for banking decisions — open source reference implementation.

Six governed layers composable by any product team through a stable SDK:

| Layer | Responsibility | Key Pattern |
| --- | --- | --- |
| **L1 Context Assembly** | Live customer profile in < 200ms | Parallel async fetch · graceful degradation |
| **L2 Vector Search** | Right policy at decision time | Hybrid dense + BM25 · RRF merge · cross-encoder rerank |
| **L3 Orchestration** | Hub-and-spoke agents · propose only | Tool authorization in code · schema-validated outputs |
| **L4 Guardrails** | REGULATORY → BUSINESS → AI sequence | Versioned YAML rules · BISG fairness · SLA approval queue |
| **L5 A/B + Model Gov.** | Deterministic experiments + drift | Hash-based assignment · champion/challenger · PSI/KS/recall |
| **L6 SDK + Execution** | Product team surface | Blueprint catalog · outcome capture · trace_id threading |

**One `trace_id` reconstructs every decision for regulatory replay.**

```bash
git clone https://github.com/saralabiswal/banking-agentic-ai-platform
cd banking-agentic-ai-platform && make install && make docker-up
cp .env.example .env && make demo
# Runs end-to-end — no API key required
```

[![Python](https://img.shields.io/badge/Python-3.12-3b82f6?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.111-10b981?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/React-18-61dafb?style=flat-square&logo=react&logoColor=white)](https://react.dev)
[![Qdrant](https://img.shields.io/badge/Qdrant-vector--store-dc2626?style=flat-square)](https://qdrant.tech)
[![MLflow](https://img.shields.io/badge/MLflow-registry-f59e0b?style=flat-square)](https://mlflow.org)
[![License](https://img.shields.io/badge/license-MIT-a855f7?style=flat-square)](LICENSE)

---

### 🧪 [AgentOps Evaluation Framework](https://github.com/saralabiswal/agentops-eval-llmops)

> Evaluation harness for governed LLM agents — because production AI without evals is just a demo you shipped.

Most agentic AI systems stop at building the agent. This framework answers the question every production deployment eventually faces: **how do you know it's still working correctly next month?**

| Component | What it does |
| --- | --- |
| **YAML test cases** | Benchmark scenarios for payment risk, billing disputes, churn prevention |
| **Independent judge** | Separate judge backend (mock / Ollama / LiteLLM) — not the same model being evaluated |
| **Scoring dimensions** | Faithfulness · relevance · context precision · consistency · composite quality gate |
| **SUT backends** | Mock · Ollama · cloud API · banking platform adapter — swap without changing test cases |
| **Reports** | HTML + JSON · SSE streaming · side-by-side model comparison |

Designed to plug directly into the banking platform as its evaluation layer — same `trace_id`, same scenarios, same policy boundaries.

```bash
make install && cp .env.example .env
make demo                         # mock backend, no API key required
make dev                          # API → http://localhost:8001
```

[![Python](https://img.shields.io/badge/Python-3.12-3b82f6?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.111-10b981?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![LiteLLM](https://img.shields.io/badge/LiteLLM-multi--provider-6366f1?style=flat-square)](https://litellm.ai)
[![Ollama](https://img.shields.io/badge/Ollama-local-0ea5e9?style=flat-square)](https://ollama.com)

---

## Production Platforms (Oracle, 2009–Present)

| Agentic AI on CPQ | Unity CDP AI/ML Platform |
| --- | --- |
| **MCP-powered multi-agent orchestration** | **6 production models · 9,000+ customers · day-one GA** |
| Renewal Agent — autonomous risk scoring + optimized proposal generation | Next Best Action / Offer |
| Quote Generation Agent — real-time margin enforcement + cross-sell intelligence | Churn & Engagement Propensity |
| AI Agent Studio — agent lifecycle, tool routing, policy enforcement across the full commercial lifecycle | Customer Lifetime Value (CLV) |
| Cross-vendor CRM integration layer: Salesforce + MS Dynamics 365 → Oracle CPQ Cloud + Fusion OM + Subscription Management | RFM Segmentation |
| | Multi-Touch Attribution (MTA) |
| | Media Mix Modeling (MMM) |
| **30% renewal cycle compression · 28% quote processing improvement** | Full MLOps stack: feature stores · training pipelines · real-time + batch inference · embedding pipelines · vector DBs · drift detection · responsible AI governance |

---

## Open Source Portfolio

| Layer | Repo | What it demonstrates |
| --- | --- | --- |
| **Platform** | [banking-agentic-ai-platform](https://github.com/saralabiswal/banking-agentic-ai-platform) | 6-layer governed agentic pipeline · guardrails · A/B · full audit |
| **Platform** | [agentic-cdp-mlops](https://github.com/saralabiswal/agentic-cdp-mlops) | 8-stage ML platform · model registry · governed promotion lifecycle |
| **Ops** | [agentops-eval-llmops](https://github.com/saralabiswal/agentops-eval-llmops) | LLM agent evaluation · judge/SUT separation · faithfulness scoring |
| **Domain Agent** | [agentic-revenue-cpq](https://github.com/saralabiswal/agentic-revenue-cpq) | MCP integration · LangGraph · Oracle CPQ-style quote lifecycle |
| **Domain Agent** | [agentic-saas-renewal](https://github.com/saralabiswal/agentic-saas-renewal) | Guarded LLM decisioning · ML risk scoring · full evidence audit |
| **Domain Agent** | [agentic-hr-onboarding-mcp](https://github.com/saralabiswal/agentic-hr-onboarding-mcp) | MCP connectors · Workday/Jira/Slack/Salesforce · idempotency |
| **Domain Agent** | [agentic-ecommerce-rag](https://github.com/saralabiswal/agentic-ecommerce-rag) | RAG · LangGraph · multi-agent · quality gate · human feedback |

---

## Technical Skills

**AI / ML / Agentic**

![GenAI](https://img.shields.io/badge/Generative%20AI-3b82f6?style=flat-square)
![Agentic AI](https://img.shields.io/badge/Agentic%20AI-3b82f6?style=flat-square)
![LLMs](https://img.shields.io/badge/LLMs-3b82f6?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-3b82f6?style=flat-square)
![MCP](https://img.shields.io/badge/MCP%20Dev%20%26%20Integration-3b82f6?style=flat-square)
![LangChain](https://img.shields.io/badge/LangChain-3b82f6?style=flat-square)
![LangGraph](https://img.shields.io/badge/LangGraph-3b82f6?style=flat-square)
![MLOps](https://img.shields.io/badge/MLOps-3b82f6?style=flat-square)
![LLMOps](https://img.shields.io/badge/LLMOps-3b82f6?style=flat-square)
![Responsible AI](https://img.shields.io/badge/Responsible%20AI-3b82f6?style=flat-square)
![Vector DBs](https://img.shields.io/badge/Vector%20Databases-3b82f6?style=flat-square)

**Languages & Frameworks**

[![Python](https://img.shields.io/badge/Python-3776ab?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![Java](https://img.shields.io/badge/Java-f89820?style=flat-square&logo=openjdk&logoColor=white)](https://java.com)
[![SQL](https://img.shields.io/badge/SQL-4479a1?style=flat-square&logo=postgresql&logoColor=white)](https://postgresql.org)
[![Apache Spark](https://img.shields.io/badge/Apache%20Spark-e25a1c?style=flat-square&logo=apachespark&logoColor=white)](https://spark.apache.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61dafb)](https://react.dev)

**Cloud & Infrastructure**

[![OCI](https://img.shields.io/badge/OCI-f80000?style=flat-square&logo=oracle&logoColor=white)](https://oracle.com/cloud)
[![AWS](https://img.shields.io/badge/AWS-232f3e?style=flat-square&logo=amazonaws&logoColor=white)](https://aws.amazon.com)
[![GCP](https://img.shields.io/badge/GCP-4285f4?style=flat-square&logo=googlecloud&logoColor=white)](https://cloud.google.com)
[![Azure](https://img.shields.io/badge/Azure-0078d4?style=flat-square&logo=microsoftazure&logoColor=white)](https://azure.microsoft.com)
[![Docker](https://img.shields.io/badge/Docker-2496ed?style=flat-square&logo=docker&logoColor=white)](https://docker.com)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-326ce5?style=flat-square&logo=kubernetes&logoColor=white)](https://kubernetes.io)

**Data & ML Stack**

[![Kafka](https://img.shields.io/badge/Kafka-231f20?style=flat-square&logo=apachekafka&logoColor=white)](https://kafka.apache.org)
[![Qdrant](https://img.shields.io/badge/Qdrant-dc2626?style=flat-square)](https://qdrant.tech)
[![MLflow](https://img.shields.io/badge/MLflow-0194e2?style=flat-square)](https://mlflow.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-ff6f00?style=flat-square&logo=tensorflow&logoColor=white)](https://tensorflow.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?style=flat-square&logo=pytorch&logoColor=white)](https://pytorch.org)
[![HuggingFace](https://img.shields.io/badge/Hugging%20Face-ffd21e?style=flat-square)](https://huggingface.co)

---

## By the Numbers

| | |
| --- | --- |
| **17+** years production AI experience | **40+** person global org (US + India) |
| **9,000+** customers at day-one platform launch | **600+** enterprise clients in production |
| **50+** countries served | **6** production ML models at GA |
| **30%** renewal cycle compression | **28%** quote processing efficiency improvement |
| **2x** internal promotion rate increase | **32%** incident volume reduction |

---

## Certifications

[![Deep Learning](https://img.shields.io/badge/Deep%20Learning%20Specialization-DeepLearning.AI%20%2F%20Coursera-0056d2?style=flat-square&logo=coursera&logoColor=white)](https://www.coursera.org/account/accomplishments/specialization/certificate/PH7HB89PB4H2)

[![MLOps](https://img.shields.io/badge/ML%20Engineering%20for%20Production%20(MLOps)-DeepLearning.AI%20%2F%20Coursera-0056d2?style=flat-square&logo=coursera&logoColor=white)](https://www.coursera.org/account/accomplishments/specialization/certificate/Z63Q5RRGD92F)

---

## Education

- **Post Graduate Diploma, Machine Learning** — Cornell University, NY
- **MBA, Technology Management** — University of Phoenix, AZ
- **B.S., Computer Science & Engineering** — Utkal University, India

---

I build the platforms that make AI commercially accountable — not just technically impressive.

**Industries:** Enterprise SaaS · AI-native companies · Revenue / GTM platforms · CDPs · B2B tech · Agentic AI infrastructure

---

**Open to conversations about AI platform architecture, agentic AI systems, and engineering leadership.**

[![LinkedIn](https://img.shields.io/badge/Connect%20on%20LinkedIn-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal)
[![Email](https://img.shields.io/badge/saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)
