# Sarala Biswal

**VP / Director of AI Engineering · AI Platform Architect · Agentic AI · MCP · MLOps · Enterprise Scale · Oracle CPQ · Quote-to-Cash**

*Belmont, CA · He/Him*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-saralabiswal-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal)
[![Email](https://img.shields.io/badge/Email-saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)
[![Profile Views](https://komarev.com/ghpvc/?username=saralabiswal&style=flat-square&color=3b82f6&label=Profile+Views)](https://github.com/saralabiswal)

# Sarala Biswal

**VP / Director of Engineering · Agentic AI · MCP · MLOps · CPQ · Quote-to-Cash · Hands-On Technical Leader**

*Belmont, CA · He/Him*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-saralabiswal-0a66c2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/saralabiswal)
[![Email](https://img.shields.io/badge/Email-saralabiswal%40gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:saralabiswal@gmail.com)
[![Blog](https://img.shields.io/badge/Blog-nlpml.ai-3b82f6?style=flat-square)](https://nlpml.ai)
[![Profile Views](https://komarev.com/ghpvc/?username=saralabiswal&style=flat-square&color=3b82f6&label=Profile+Views)](https://github.com/saralabiswal)

---

## About

I build AI/ML platforms that generate revenue — not just predictions.
Hands-on engineering leader who architects and codes production systems personally
while setting technical direction for a 40+ person global org.

17+ years at Oracle shipping two flagship AI platforms at enterprise scale:

- **Agentic AI on CPQ** — Renewal Agent + Quote Generation Agent · 3,000+ active sales users · 600+ enterprise clients · 50+ countries · 30% renewal cycle compression · 28% quote processing efficiency improvement
- **Unity CDP AI/ML** — 6 production models (Next Best Action, Churn Propensity, CLV, RFM Segmentation, Multi-Touch Attribution, MMM) · 9,000+ customers at day-one GA · no phased rollout

The hard part isn't the model — it's the integration layer. I solved the cross-vendor problem in production: unified live context from Salesforce, MS Dynamics 365, and Oracle clouds so agents make decisions on real data, not cached snapshots.

---

## Featured Projects

### 🔗 [agentic-mcp-quote-to-cash](https://github.com/saralabiswal/agentic-mcp-quote-to-cash)

> MCP-powered integration layer for vendor-agnostic quote-to-cash agentic decisions — the cross-vendor architecture pattern running in production across 600+ enterprise clients.

**The core proof: vendor selection is configuration, not agent code.** Switching CRM from Salesforce to Microsoft Dynamics 365, or Order Management from Oracle FOM to SAP S/4HANA, changes the adapter path and source attribution — the decision agent and canonical schema are untouched.

| Slot | Adapter implementations | Canonical output |
|---|---|---|
| **CRM** | Salesforce · MS Dynamics 365 · Oracle CX Sales | Account · Opportunity · Contact · Activity |
| **CPQ** | Oracle CPQ Cloud | Product · PriceBook · Quote |
| **Order Management** | Oracle FOM · Salesforce OMS · SAP S/4HANA · Zuora · NetSuite | Order · OrderLine · FulfillmentStatus |
| **Subscription** | Oracle Sub Cloud · Zuora · Chargebee · Salesforce Revenue Cloud | Subscription · UsageHealth · RenewalSignal |
| **Install Base** | Oracle Install Base · Salesforce Asset · ServiceNow CMDB | InstalledProduct · Entitlement |

**16 adapters. 5 commercial-system slots. One canonical schema. Seven demo scenarios.**

```bash
git clone https://github.com/saralabiswal/agentic-mcp-quote-to-cash
cd agentic-mcp-quote-to-cash && make install && make seed
make dev-api          # FastAPI → http://localhost:8000
cd ui && npm install && npm run dev -- --port 3001
# No API key required — runs end-to-end in demo mode
```

[![Python](https://img.shields.io/badge/Python-3.12-3b82f6?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.111-10b981?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![MCP SDK](https://img.shields.io/badge/MCP%20SDK-1.0-a855f7?style=flat-square)](https://github.com/modelcontextprotocol)
[![Pydantic v2](https://img.shields.io/badge/Pydantic-v2-e11d48?style=flat-square)](https://docs.pydantic.dev)
[![React](https://img.shields.io/badge/React-18-61dafb?style=flat-square&logo=react&logoColor=white)](https://react.dev)
[![License](https://img.shields.io/badge/license-MIT-f59e0b?style=flat-square)](LICENSE)

---

### 🏦 [agentic-banking-llmops](https://github.com/saralabiswal/agentic-banking-llmops)

> Production-grade, cloud-agnostic Agentic AI platform for banking decisions — open source reference implementation of the engineering disciplines that separate trustworthy AI from demos that don't survive contact with production.

Six governed layers composable by any product team through a stable SDK:

| Layer | Responsibility | Key Pattern |
|---|---|---|
| **L1 Context Assembly** | Live customer profile in < 200ms | Parallel async fetch · long-term memory · graceful degradation |
| **L2 Vector Search** | Right policy at decision time | Hybrid dense + BM25 · RRF merge · cross-encoder rerank |
| **L3 Orchestration** | Hub-and-spoke agents · propose only | Tool authorization in code · schema-validated outputs |
| **L4 Guardrails** | REGULATORY → BUSINESS → AI sequence | Versioned YAML rules · BISG fairness · SLA approval queue |
| **L5 A/B + Model Gov.** | Deterministic experiments + drift | Hash-based assignment · champion/challenger · PSI/KS/recall |
| **L6 SDK + Execution** | Product team surface | Blueprint catalog · outcome capture · trace_id threading |

**One `trace_id` reconstructs every decision for regulatory replay.**
**4-gate offline evaluation: benchmark · fairness · Adverse Impact Ratio · LLM-judge.**

```bash
git clone https://github.com/saralabiswal/agentic-banking-llmops
cd agentic-banking-llmops && make install && make docker-up
cp .env.example .env && make demo
# Runs end-to-end — no API key required
```

[![Python](https://img.shields.io/badge/Python-3.12-3b82f6?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.111-10b981?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/React-18-61dafb?style=flat-square&logo=react&logoColor=white)](https://react.dev)
[![Qdrant](https://img.shields.io/badge/Qdrant-vector--store-dc2626?style=flat-square)](https://qdrant.tech)
[![MLflow](https://img.shields.io/badge/MLflow-registry-f59e0b?style=flat-square)](https://mlflow.org)
[![Coverage](https://img.shields.io/badge/coverage-90%25%2B-22c55e?style=flat-square)](https://pytest.org)
[![License](https://img.shields.io/badge/license-MIT-a855f7?style=flat-square)](LICENSE)

---

### 🧪 [agentops-eval-llmops](https://github.com/saralabiswal/agentops-eval-llmops)

> Evaluation harness for governed LLM agents — because production AI without evals is just a demo you shipped.

Most agentic AI systems stop at building the agent. This framework answers the question every production deployment eventually faces: **how do you know it's still working correctly next month?**

| Component | What it does |
|---|---|
| **YAML test cases** | Benchmark scenarios for payment risk, billing disputes, churn prevention |
| **Independent judge** | Separate judge backend — not the same model being evaluated (prevents self-evaluation bias) |
| **Scoring dimensions** | Faithfulness · answer relevance · context precision · consistency · latency/quality tradeoff |
| **SUT backends** | Mock · Ollama · cloud API · banking platform adapter — swap without changing test cases |
| **Reports** | HTML + JSON · SSE streaming · side-by-side model comparison |

Plugs directly into `agentic-banking-llmops` as its evaluation layer — same `trace_id`, same scenarios, same policy boundaries.

```bash
make install && cp .env.example .env
make demo                         # mock backend, no API key required
make dev                          # API → http://localhost:8001
```

[![Python](https://img.shields.io/badge/Python-3.12-3b82f6?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.111-10b981?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![LiteLLM](https://img.shields.io/badge/LiteLLM-multi--provider-6366f1?style=flat-square)](https://litellm.ai)
[![Ollama](https://img.shields.io/badge/Ollama-local--first-0ea5e9?style=flat-square)](https://ollama.com)

---

### 📊 [agentic-llm-observability](https://github.com/saralabiswal/agentic-llm-observability)

> Production LLMOps control plane for Quote-to-Cash agentic workflows — token cost attribution, quality scoring, latency SLOs, prompt versioning, and semantic drift detection across five providers.

Answers the production questions most enterprises cannot answer:

| Question | What the platform tracks |
|---|---|
| How much did this agent run cost? | Token cost per call · per model · per use case · per provider |
| Which model and prompt version ran? | Prompt version registry · A/B comparison · rollout history |
| Did quality stay above threshold? | Faithfulness · relevance · coherence · hallucination signals · quality gates |
| Were latency SLOs met? | p50 / p95 / p99 per model · SLO compliance % · breach visibility |
| Did outputs drift from baseline? | Semantic drift score · threshold alerts · operational posture |

**Five providers with real rate cards:**

| Provider | Model | Use case |
|---|---|---|
| Local LLM | Ollama — Llama 3.2 · Qwen 2.5 · Mistral | Actual execution — standalone, no API key |
| AWS Bedrock | Claude 3.5 Haiku | Production agent workloads |
| Azure OpenAI | GPT-4o mini | Global deployment, low-cost reasoning |
| OCI Generative AI | Cohere Command R | Enterprise RAG-style flows |
| Google Vertex AI | Gemini 2.0 Flash | Fast agentic workflows |

```bash
make install && make seed
ollama pull llama3.2              # default local model
make dev-api                      # API → http://localhost:9100
make dev-ui                       # UI  → http://localhost:5173
# No API key required
```

[![Python](https://img.shields.io/badge/Python-3.12-3b82f6?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.111-10b981?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Ollama](https://img.shields.io/badge/Ollama-local--first-f59e0b?style=flat-square)](https://ollama.com)
[![OCI](https://img.shields.io/badge/OCI-Generative%20AI-f87171?style=flat-square&logo=oracle&logoColor=white)](https://oracle.com/cloud)
[![React](https://img.shields.io/badge/React-18-61dafb?style=flat-square&logo=react&logoColor=white)](https://react.dev)

---

## Production Platforms (Oracle, 2009–Present)

| Agentic AI on CPQ | Unity CDP AI/ML Platform |
|---|---|
| **MCP-powered multi-agent orchestration** | **6 production models · 9,000+ customers · day-one GA** |
| Renewal Agent — autonomous risk scoring + optimized proposal generation | Next Best Action / Offer |
| Quote Generation Agent — real-time margin enforcement + cross-sell intelligence | Churn & Engagement Propensity |
| AI Agent Studio — agent lifecycle, tool routing, policy enforcement across the full commercial lifecycle | Customer Lifetime Value (CLV) |
| Cross-vendor CRM integration layer: Salesforce + MS Dynamics 365 → Oracle CPQ Cloud + Fusion Order Management + Subscription Management · [Reference implementation →](https://github.com/saralabiswal/agentic-mcp-quote-to-cash) | RFM Segmentation |
| | Multi-Touch Attribution (MTA) |
| | Media Mix Modeling (MMM) |
| **30% renewal cycle compression · 28% quote processing improvement** | Full MLOps stack: feature stores · training pipelines (TensorFlow · PyTorch · Hugging Face) · real-time + batch inference · embedding pipelines · vector DBs · RAG · drift detection · responsible AI governance |

---

## Open Source Portfolio

| Layer | Repo | What it demonstrates |
|---|---|---|
| **Integration** | [agentic-mcp-quote-to-cash](https://github.com/saralabiswal/agentic-mcp-quote-to-cash) | 16 MCP adapters · cross-vendor live context · CRM-agnostic · Quote-to-Cash lifecycle |
| **Platform** | [agentic-banking-llmops](https://github.com/saralabiswal/agentic-banking-llmops) | 6-layer governed agentic pipeline · guardrails · A/B · regulatory replay · 90% coverage |
| **Platform** | [agentic-cdp-mlops](https://github.com/saralabiswal/agentic-cdp-mlops) | 8-stage ML platform · 4 models · model registry · governed promotion lifecycle |
| **Ops** | [agentops-eval-llmops](https://github.com/saralabiswal/agentops-eval-llmops) | LLM agent evaluation · judge/SUT separation · faithfulness · quality gates |
| **Ops** | [agentic-llm-observability](https://github.com/saralabiswal/agentic-llm-observability) | LLMOps control plane · token cost · quality · latency SLOs · 5 providers |
| **Domain** | [agentic-revenue-cpq](https://github.com/saralabiswal/agentic-revenue-cpq) | MCP integration · LangGraph · Oracle CPQ-style quote lifecycle |
| **Domain** | [agentic-hr-onboarding-mcp](https://github.com/saralabiswal/agentic-hr-onboarding-mcp) | MCP connectors · Workday/Jira/Slack/Salesforce · idempotency |
| **Domain** | [agentic-ecommerce-rag](https://github.com/saralabiswal/agentic-ecommerce-rag) | RAG · LangGraph · multi-agent · quality gate · human feedback |

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
|---|---|
| **17+** years production AI/ML experience | **40+** person global org (US + India) |
| **9,000+** customers at day-one platform launch | **600+** enterprise clients in production |
| **50+** countries served | **6** production ML models shipped at GA |
| **3,000+** active sales users on agentic platform | **16** MCP adapters across 5 vendor slots |
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

*I build the platforms that make AI commercially accountable — not just technically impressive.*
