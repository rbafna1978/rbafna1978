<div align="center">

# hey, I'm Rishit 👋

**MS CS @ Arizona State · Backend & Distributed Systems · Available for SWE Internships**

Mumbai → Tempe, AZ &nbsp;·&nbsp; [rishitbafna.vercel.app](https://rishitbafna.vercel.app) &nbsp;·&nbsp; [linkedin](https://linkedin.com/in/rishit-bafna) &nbsp;·&nbsp; [bafnarishit@gmail.com](mailto:bafnarishit@gmail.com)

</div>

---

I build things that hold up under pressure. Not just prototypes — production-grade systems with real constraints: sub-50ms p99 latency, 0.17% class imbalance, zero data loss on leader failover. I care about correctness before speed, and I'll argue for a well-tested monolith over a prematurely distributed mess any day.

Currently deep in distributed systems and ML pipelines. Also: Formula 1 fan, chai enthusiast, and someone who has definitely read the Raft paper more times than is healthy.

---

## what I've built

**[RiskStream](https://github.com/rbafna1978/riskstream)** — end-to-end fraud detection over 500K+ transactions. XGBoost + Isolation Forest, point-in-time-correct features (no label leakage), p99 inference under 50ms with zero hot-path DB reads. PSI-based drift monitoring self-retrains and hot-swaps models without restarting the service.
`Python · XGBoost · FastAPI · PostgreSQL · Redis · MLflow · Docker`

**[CyberSentient RAG Pipeline](https://github.com/rbafna1978/cybersentient-rag)** — hybrid retrieval over 100K+ CVE/CWE/CAPEC records. Dense vectors + BM25 sparse retrieval + Reciprocal Rank Fusion, cross-encoder reranked with Qwen3-Reranker-8B. 400ms end-to-end across a 6-feed ingestion pipeline.
`Python · Qwen3-Embedding-8B · Qdrant · BM25 · FastAPI`

**[Distributed Key-Value Store](https://github.com/rbafna1978/distributed-kv-store)** — Raft consensus from scratch. 5-node cluster, gRPC transport, sub-5ms reads, chaos-tested leader failover with zero data loss. Built this because I wanted to understand the protocol, not just cite the paper.
`Java · Raft · gRPC · Protocol Buffers · Docker`

**[AI Interview Coach](https://interview-helper-three.vercel.app)** — browser-native voice transcription, STAR structure scoring, real-time filler word detection. Behavioral, technical, and freestyle modes with session history.
`React · Web Speech API · Node.js · PostgreSQL`

**[GitHub Dependency Visualizer](https://github.com/rbafna1978/github-dependency-visualizer)** — parses `package.json`, `pom.xml`, `go.mod` across repos into an interactive force-directed graph. Detects circular deps and version conflicts.
`React · TypeScript · Node.js · Cytoscape`

**[Multithreaded HTTP Server](https://github.com/rbafna1978/http-server)** — socket programming + custom thread pool in C++, built from scratch. No frameworks, no shortcuts.
`C++ · Sockets · Multithreading`

---

## where I've shipped

**J. Miller Custom Cues** *(SWE Intern, Aug–Dec 2025)* — built a production 3D product configurator in Three.js + React, cutting customer revision cycles by 35%. Wired up a PostgreSQL REST API with Stripe integration handling 100+ orders at sub-200ms response times.

**Winssoft Technologies** *(SWE Intern, May–Jul 2025)* — rewrote SQL queries over 200K+ records using composite indexes and materialized views, slashing dashboard load from 8s to under 2s. Refactored a payment microservice (5K+ daily txns) with idempotency guarantees to eliminate duplicate charges.

---

## stack

```
Languages   Python · Java · TypeScript · JavaScript · C++ · SQL · Go
Backend     FastAPI · Node.js · Express · gRPC · WebSockets · REST
Frontend    React · Next.js · Three.js · Tailwind
Data & ML   PostgreSQL · Redis · Kafka · XGBoost · PyTorch · Qdrant · MLflow
Infra       Docker · AWS (S3, EC2) · Linux · Git
```

---

## papers I've actually read

- Raft: In Search of an Understandable Consensus Algorithm — Ongaro & Ousterhout (2014)
- Dynamo: Amazon's Highly Available Key-value Store — DeCandia et al. (2007)
- Bigtable: A Distributed Storage System for Structured Data — Chang et al. (2006)
- MapReduce: Simplified Data Processing on Large Clusters — Dean & Ghemawat (2004)
- The Google File System — Ghemawat, Gobioff & Leung (2003)

---

<div align="center">

**Open to SWE internships in backend, distributed systems, and ML infra.**

[bafnarishit@gmail.com](mailto:bafnarishit@gmail.com) &nbsp;·&nbsp; [rishitbafna.vercel.app](https://rishitbafna.vercel.app) &nbsp;·&nbsp; Tempe, AZ

</div>
