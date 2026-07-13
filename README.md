# Sarala Biswal

**VP / Director of AI Engineering · Agentic AI · MCP · MLOps · CPQ · Quote-to-Cash · Hands-On Technical Leader**

*Belmont, CA · He/Him*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-saralabiswal-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal)
[![Email](https://img.shields.io/badge/Email-saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)
[![Blog](https://img.shields.io/badge/Blog-nlpml.ai-3b82f6?style=flat-square)](https://nlpml.ai)
[![Profile Views](https://komarev.com/ghpvc/?username=saralabiswal&style=flat-square&color=3b82f6&label=Profile+Views)](https://github.com/saralabiswal)

---

## About

I build AI/ML platforms that generate revenue — not just predictions.
Hands-on engineering leader who architects production systems personally while setting technical direction for a global org.

17+ years at Oracle shipping two flagship AI platforms at enterprise scale:

- **Agentic AI on CPQ** — Renewal Agent + Quote Generation Agent · 3,000+ sales users · 600+ enterprise clients · 50+ countries · 30% renewal cycle compression · 28% quote processing efficiency improvement
- **Unity CDP AI/ML** — 6 production models (Next Best Action, Churn Propensity, CLV, RFM Segmentation, Multi-Touch Attribution, MMM) · 9,000+ customers at day-one GA · no phased rollout

The hard part isn't the model — it's the integration layer and the management layer around it. I solved the cross-vendor problem in production: unified live context from Salesforce, MS Dynamics, and Oracle clouds so agents make decisions on real data, not cached snapshots. And I've built what most companies are now hiring specialists to operate: agent tracing, cost attribution, quality scoring, and governed promotion — **AgentOps as a discipline, not an afterthought.**

---

## Start Here — 3 Repos That Define The Portfolio

These three show the full arc: govern the agent, prove the integration pattern, prove it holds up in a regulated domain.

### 🎛️ [AgentOps Control Plane](https://github.com/saralabiswal/agentops-control-plane)
> *"An agent that can't be traced, costed, or tied to an outcome isn't a production system. It's a demo with uptime."*

Traces every agent run, attributes LLM cost, scores output quality asynchronously, and maps decisions to financial outcomes. Seven business agents across Project Management and Revenue Management, one enforced management-layer contract. This is the category — AgentOps — built as infrastructure, not a slide.

`FastAPI` `LangGraph` `React` `SQLite` `MLflow`

### 🔗 [Agentic MCP Quote-to-Cash](https://github.com/saralabiswal/agentic-mcp-quote-to-cash)
Vendor-agnostic quote-to-cash decisioning — MCP adapters assemble live CRM, CPQ, Order Management, Subscription, and Install Base context into one canonical schema. Swap Salesforce for Dynamics and the agent code doesn't change. 16 adapters, 7 demo scenarios, full audit trail.

`Python` `React` `MCP` `Pydantic v2`

### ⚖️ [Agentic Regulated Decisioning](https://github.com/saralabiswal/agentic-regulated-decisioning)
Domain-independent L0–L9 platform for regulated AI decisions — insurance, lending, healthcare, and wealth run on the same runtime with zero domain-specific imports in platform code. Jurisdiction-aware governance, append-only audit, human review workbench.

`LangGraph` `MCP` `MLflow` `Redis Streams` `PostgreSQL`

---

## Full Portfolio — 13 Repos by Category

### AgentOps & Governance Infrastructure
*The category itself — observability, cost, quality, and evaluation for agents already in production*

| Repo | What it proves |
|---|---|
| [agentops-control-plane](https://github.com/saralabiswal/agentops-control-plane) | Agent tracing, LLM cost attribution, async quality scoring, financial outcome mapping |
| [agentic-llm-observability](https://github.com/saralabiswal/agentic-llm-observability) | Quote-to-Cash LLMOps control plane — token economics, latency SLOs, prompt versioning, semantic drift |
| [agentops-eval-llmops](https://github.com/saralabiswal/agentops-eval-llmops) | LLM agent evaluation — faithfulness, relevance, consistency, judge/SUT separation |

### Enterprise Agentic Systems by Domain
*Proof the integration and governance patterns hold across industries*

| Repo | Domain | What it proves |
|---|---|---|
| [agentic-mcp-quote-to-cash](https://github.com/saralabiswal/agentic-mcp-quote-to-cash) | Revenue / CPQ | Cross-vendor MCP integration, live context assembly, vendor-swap without code change |
| [agentic-banking-llmops](https://github.com/saralabiswal/agentic-banking-llmops) | Banking | 6-layer governed pipeline, regulatory replay, drift monitoring, closed feedback loop |
| [agentic-regulated-decisioning](https://github.com/saralabiswal/agentic-regulated-decisioning) | Insurance / Lending / Healthcare / Wealth | Domain-as-plugin architecture, jurisdiction-aware governance, append-only audit |
| [agentic-saas-renewal](https://github.com/saralabiswal/agentic-saas-renewal) | SaaS Revenue | Hybrid rules + ML decisioning, validator-gated LLM participation, MLOps lifecycle |
| [agentic-revenue-cpq](https://github.com/saralabiswal/agentic-revenue-cpq) | CPQ | Multi-agent quoting, LangGraph orchestration, RAG-backed product knowledge |
| [agentic-cdp-mlops](https://github.com/saralabiswal/agentic-cdp-mlops) | Customer Data Platform | 8-stage ML platform, model registry, governed promotion lifecycle |
| [agentic-hr-onboarding-mcp](https://github.com/saralabiswal/agentic-hr-onboarding-mcp) | HR Ops | MCP connectors across Workday/Jira/Slack/Salesforce, idempotency, audit log |
| [agentic-ecommerce-rag](https://github.com/saralabiswal/agentic-ecommerce-rag) | E-commerce | RAG with quality gates, competitor analysis, human-in-the-loop review |

### Core ML Foundations
*Production ML discipline underneath the agent layer*

| Repo | What it proves |
|---|---|
| [learning-to-rank-distillation](https://github.com/saralabiswal/learning-to-rank-distillation) | Governed ranking lifecycle — teacher/student distillation, fairness trade-offs, executable promotion gates |

### Book
| Repo | What it is |
|---|---|
| [production-ai-architecture](https://github.com/saralabiswal/production-ai-architecture) | Companion code for *Production AI Architecture* (Amazon) — gateways, RAG, agent workflows, evaluation harnesses, governance pipelines |

---

## Technical Skills

**AI / ML / Agentic**

![GenAI](https://img.shields.io/badge/GenAI-3b82f6?style=flat-square) ![Agentic AI](https://img.shields.io/badge/Agentic%20AI-3b82f6?style=flat-square) ![LLMs](https://img.shields.io/badge/LLMs-3b82f6?style=flat-square) ![RAG](https://img.shields.io/badge/RAG-3b82f6?style=flat-square) ![MCP](https://img.shields.io/badge/MCP%20Dev%20%26%20Integration-3b82f6?style=flat-square) ![LangChain](https://img.shields.io/badge/LangChain-3b82f6?style=flat-square) ![LangGraph](https://img.shields.io/badge/LangGraph-3b82f6?style=flat-square) ![MLOps](https://img.shields.io/badge/MLOps-3b82f6?style=flat-square) ![AgentOps](https://img.shields.io/badge/AgentOps-3b82f6?style=flat-square) ![Responsible AI](https://img.shields.io/badge/Responsible%20AI-3b82f6?style=flat-square) ![Vector DBs](https://img.shields.io/badge/Vector%20Databases-3b82f6?style=flat-square)

**Languages & Frameworks**

![Python](https://img.shields.io/badge/Python-3776ab?style=flat-square&logo=python&logoColor=white) ![Java](https://img.shields.io/badge/Java-f89820?style=flat-square&logo=openjdk&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479a1?style=flat-square&logo=postgresql&logoColor=white) ![Apache Spark](https://img.shields.io/badge/Apache%20Spark-e25a1c?style=flat-square&logo=apachespark&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![React](https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61dafb)

**Cloud & Infrastructure**

![OCI](https://img.shields.io/badge/OCI-f80000?style=flat-square&logo=oracle&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232f3e?style=flat-square&logo=amazonaws&logoColor=white) ![GCP](https://img.shields.io/badge/GCP-4285f4?style=flat-square&logo=googlecloud&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0078d4?style=flat-square&logo=microsoftazure&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ed?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326ce5?style=flat-square&logo=kubernetes&logoColor=white)

**Data & ML Stack**

![Kafka](https://img.shields.io/badge/Kafka-231f20?style=flat-square&logo=apachekafka&logoColor=white) ![Qdrant](https://img.shields.io/badge/Qdrant-dc2626?style=flat-square) ![MLflow](https://img.shields.io/badge/MLflow-0194e2?style=flat-square) ![TensorFlow](https://img.shields.io/badge/TensorFlow-ff6f00?style=flat-square&logo=tensorflow&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?style=flat-square&logo=pytorch&logoColor=white) ![HuggingFace](https://img.shields.io/badge/HuggingFace-ffd21e?style=flat-square)

---

## By The Numbers

| | |
|---|---|
| **17+** years engineering leadership | **13** open-source reference architecture repos |
| **9,000+** customers at day-one platform launch | **600+** enterprise clients in production |
| **50+** countries served | **6** production ML models at GA |
| **30%** renewal cycle compression | **28%** quote processing efficiency improvement |

*Note: org size and a couple of internal leadership metrics are intentionally left off this table pending a consistency pass across GitHub / LinkedIn / resume — see note below.*

---

## Certifications

[![Deep Learning Specialization](https://img.shields.io/badge/DeepLearning.AI-Deep%20Learning%20Specialization-0056d2?style=flat-square&logo=coursera&logoColor=white)](https://www.coursera.org/account/accomplishments/specialization/certificate/PH7HB89PB4H2)
[![MLOps Specialization](https://img.shields.io/badge/DeepLearning.AI-MLOps%20Specialization-0056d2?style=flat-square&logo=coursera&logoColor=white)](https://www.coursera.org/account/accomplishments/specialization/certificate/Z63Q5RRGD92F)

## Education

- **Post Graduate Diploma, Machine Learning** — Cornell University, NY
- **MBA, Technology Management** — University of Phoenix, AZ
- **B.S., Computer Science & Engineering** — Utkal University, India

---

**Where AI needs to move from a feature to core business infrastructure.**

Industries: Enterprise SaaS · AI-native companies · Revenue/GTM platforms · CDPs · B2B tech · Agentic AI infrastructure

*I build the platforms that make AI commercially accountable — not just technically impressive.*

[![LinkedIn](https://img.shields.io/badge/Connect%20on%20LinkedIn-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal) [![Email](https://img.shields.io/badge/Email-saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)
