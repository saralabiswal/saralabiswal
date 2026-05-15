

<div align="center">

# Sarala Biswal

**VP / Director of Engineering · AI/ML Platforms · Agentic AI · Enterprise Scale**

*Belmont, CA · He/Him*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-saralabiswal-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal)
[![Email](https://img.shields.io/badge/Email-saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)
[![Profile Views](https://komarev.com/ghpvc/?username=saralabiswal&style=flat-square&color=3b82f6&label=Profile+Views)](https://github.com/saralabiswal)

</div>

---

## About

I build AI/ML platforms that generate revenue — not just predictions.
Hands-on engineering leader who architects production systems personally while setting technical direction for a 40+ person global org.

17+ years at Oracle shipping two flagship AI platforms at enterprise scale:

- **Agentic AI on CPQ** — Renewal Agent + Quote Generation Agent · 3,000+ sales users · 600+ enterprise clients · 50+ countries · 30% renewal cycle compression · 28% quote processing efficiency improvement
- **Unity CDP AI/ML** — 6 production models (Next Best Action, Churn Propensity, CLV, RFM Segmentation, Multi-Touch Attribution, MMM) · 9,000+ customers at day-one GA · no phased rollout

The hard part isn't the model — it's the integration layer. I solved the cross-vendor problem in production: unified live context from Salesforce, MS Dynamics, and Oracle clouds so agents make decisions on real data, not cached snapshots.

---

## Featured Project

### 🏦 [Banking Agentic AI Platform](https://github.com/saralabiswal/banking-agentic-platform)

> A cloud-agnostic, production-grade Agentic AI platform for banking decisions — open source reference implementation.

Six governed layers composable by any product team through a stable SDK:

| Layer | Responsibility | Key Pattern |
|-------|---------------|-------------|
| **L1 Context Assembly** | Live customer profile in < 200ms | Parallel async fetch · graceful degradation |
| **L2 Vector Search** | Right policy at decision time | Hybrid dense + BM25 · RRF merge · cross-encoder rerank |
| **L3 Orchestration** | Hub-and-spoke agents · propose only | Tool authorization in code · schema-validated outputs |
| **L4 Guardrails** | REGULATORY → BUSINESS → AI sequence | Versioned YAML rules · BISG fairness · SLA approval queue |
| **L5 A/B + Model Gov.** | Deterministic experiments + drift | Hash-based assignment · champion/challenger · PSI/KS/recall |
| **L6 SDK + Execution** | Product team surface | Blueprint catalog · outcome capture · trace_id threading |

**One `trace_id` reconstructs every decision for regulatory replay.**

```bash
git clone https://github.com/saralabiswal/banking-agentic-platform
cd banking-agentic-platform && make install && make docker-up
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

## Production Platforms (Oracle, 2009–Present)

<table>
<tr>
<td width="50%" valign="top">

### Agentic AI on CPQ
**MCP-powered multi-agent orchestration**

- Renewal Agent — autonomous risk scoring + optimized proposal generation
- Quote Generation Agent — real-time margin enforcement + cross-sell intelligence
- AI Agent Studio — agent lifecycle, tool routing, policy enforcement across the full commercial lifecycle
- Cross-vendor CRM integration layer: Salesforce + MS Dynamics 365 → Oracle CPQ Cloud + Fusion OM + Subscription Management

**30% renewal cycle compression · 28% quote processing improvement**

</td>
<td width="50%" valign="top">

### Unity CDP AI/ML Platform
**6 production models · 9,000+ customers · day-one GA**

- Next Best Action / Offer
- Churn & Engagement Propensity
- Customer Lifetime Value (CLV)
- RFM Segmentation
- Multi-Touch Attribution (MTA)
- Media Mix Modeling (MMM)

Full MLOps stack: feature stores · training pipelines · real-time + batch inference · embedding pipelines · vector DBs · drift detection · responsible AI governance

</td>
</tr>
</table>

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
![Responsible AI](https://img.shields.io/badge/Responsible%20AI-3b82f6?style=flat-square)
![Vector DBs](https://img.shields.io/badge/Vector%20Databases-3b82f6?style=flat-square)

**Languages & Frameworks**

![Python](https://img.shields.io/badge/Python-3776ab?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-f89820?style=flat-square&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479a1?style=flat-square&logo=postgresql&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-e25a1c?style=flat-square&logo=apachespark&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61dafb)

**Cloud & Infrastructure**

![OCI](https://img.shields.io/badge/OCI-f80000?style=flat-square&logo=oracle&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232f3e?style=flat-square&logo=amazonaws&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285f4?style=flat-square&logo=googlecloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078d4?style=flat-square&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ed?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326ce5?style=flat-square&logo=kubernetes&logoColor=white)

**Data & ML Stack**

![Kafka](https://img.shields.io/badge/Kafka-231f20?style=flat-square&logo=apachekafka&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-dc2626?style=flat-square)
![MLflow](https://img.shields.io/badge/MLflow-0194e2?style=flat-square)
![TensorFlow](https://img.shields.io/badge/TensorFlow-ff6f00?style=flat-square&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/Hugging%20Face-ffd21e?style=flat-square)

---

## By the Numbers

<div align="center">

| | |
|:---:|:---:|
| **17+** years engineering leadership | **20+** person global org (US + India) |
| **9,000+** customers at day-one platform launch | **600+** enterprise clients in production |
| **50+** countries served | **6** production ML models at GA |
| **30%** renewal cycle compression | **28%** quote processing efficiency improvement |
| **2x** internal promotion rate increase | **32%** incident volume reduction |

</div>

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

**Where AI needs to move from a feature to core business infrastructure.**

Industries: Enterprise SaaS · AI-native companies · Revenue/GTM platforms · CDPs · B2B tech · Agentic AI infrastructure

---

<div align="center">

**Open to conversations about AI platform Architecture.**

[![LinkedIn](https://img.shields.io/badge/Connect%20on%20LinkedIn-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal)
[![Email](https://img.shields.io/badge/saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)

</div>
