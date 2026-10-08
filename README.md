# Hi, I'm Rohit Biju 👋

**Software Engineer · Cloud & Security · ML Systems · M.S. Computer Science at Northeastern University**

[LinkedIn](https://linkedin.com/in/rohitbij) · [GitHub](https://github.com/r7bb) · [Email](mailto:biju.roh@northeastern.edu)

## About Me

I'm an M.S. Computer Science student at Northeastern University's Khoury College in Boston (graduating December 2027). I like building systems that keep working when things go wrong: networks drop, events arrive out of order, services crash mid write.

Before grad school, I spent over a year at UST as an Associate in Cloud Infrastructure and Security Services, where I worked on security operations at scale, automated incident workflows, and earned a Rising Star Award.

I'm most interested in distributed systems, security engineering, cloud infrastructure, and MLOps. I'm open to internships, co ops, and full time roles.

## What I Work On

* Building realtime and offline first systems with reliable, exactly once delivery
* Designing security detection pipelines that ingest, normalize, and correlate events into incidents
* Running cloud infrastructure with a focus on availability, automation, and fast incident response
* Making ML pipelines reproducible, verifiable, and production ready

## Featured Projects

### 🛡️ [SignalForge](https://github.com/r7bb/SignalForge)
**Python · Kafka/Redpanda · OpenSearch · PostgreSQL · Next.js**

A miniature SIEM/SOC platform for security detection and response.
* Ingests host, cloud, and identity telemetry, normalizes it to OCSF, and runs Sigma detection rules
* Correlates alerts into incidents with risk scoring and MITRE ATT&CK mapping
* Handles 3,603 events/sec end to end with p95 detection latency of 0.42 ms and zero loss across 20,000 events
* At least once Kafka delivery with a dead letter queue, deduplication, tenant isolation, JWT/RBAC, and approval gated response playbooks

### 🔄 [Robis](https://github.com/r7bb/Robis)
**TypeScript · Next.js · Bun · Fastify · PostgreSQL · WebSockets · Yjs**

A collaborative workspace for issues, docs, chat, and meetings that keeps working when the network does not.
* Offline writes queue durably in IndexedDB and reconcile exactly once through client generated ids and a server idempotency ledger
* Collaborative editing with Yjs CRDTs, so two people can edit the same paragraph and both edits survive
* Realtime fan out through Postgres LISTEN/NOTIFY via a dedicated gateway: 50 subscribers at p95 8.0 ms, none dropped
* About 4,400 req/s on REST with zero errors, backed by 313 tests against real Postgres including a 25 way concurrency race

### 🛂 [Model Passport](https://github.com/r7bb/Model-Passport)
**Python · MLOps**

Wraps an ML training pipeline and produces a signed, verifiable "passport" for every trained model, recording where it came from: data, code, and training details.

### 🧬 [scPerturbAI](https://github.com/r7bb/scPerturbAI)
**Python · PyTorch · sklearn · Streamlit**

Predicts single cell transcriptional responses to unseen CRISPR perturbations.
* Trained on 111,445 cells across 237 conditions with a 5 seed MLP ensemble
* Reaches 0.92 Pearson correlation on unseen gene combinations
* Includes a Streamlit demo and a virtual screen ranking 5,022 gene pairs

### 💰 [LendWise](https://github.com/r7bb/Lendwise)
**PyTorch · sklearn · SHAP**

A two stage loan sanction model: an approval classifier chained with a separate regressor for the sanctioned amount.
* Leak proof preprocessing with transforms fitted inside cross validation folds
* Content hash dataset versioning and SHAP based feature attribution

## Experience

### Associate, Cloud Infrastructure and Security Services · UST
*2024 to 2025*
* Supported security operations handling 10,000+ incidents a month within a 15 minute SLA
* Cut mean time to resolution by 35% while maintaining 99.9% availability
* Reduced manual work by 75% through automation and built an NLP workflow reaching 87% accuracy
* Received the **Rising Star Award**

## Technical Toolbox

**Languages:** Python · TypeScript · JavaScript · SQL

**Backend & Systems:** Fastify · Bun · Next.js · PostgreSQL · Kafka/Redpanda · WebSockets · OpenSearch · REST APIs

**Cloud & DevOps:** Google Cloud · Docker · GitHub Actions · CI/CD · Linux · Prometheus

**Security:** SIEM/SOC workflows · Sigma rules · OCSF · MITRE ATT&CK · RBAC · JWT · Argon2id

**ML & Data:** PyTorch · sklearn · SHAP · Streamlit · MLOps

## Certifications & Recognition

* ☁️ Google Cloud Associate Cloud Engineer
* ⚙️ GitHub Actions Certification
* 📈 McKinsey Forward Program
* 📄 Author, Multimodal Video Keyword Search, AIP Conference Proceedings Vol. 3134 (2024), Scopus indexed
* 🏆 Rising Star Award, UST
* 🏛️ Senator, Graduate Student Government, Northeastern University

## Let's Connect

Always happy to talk about distributed systems, security engineering, cloud infrastructure, or MLOps. Reach out on [LinkedIn](https://linkedin.com/in/rohitbij) or email me at [biju.roh@northeastern.edu](mailto:biju.roh@northeastern.edu).
