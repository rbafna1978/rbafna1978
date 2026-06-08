<div align="center">

```
 ██████╗ ██╗███████╗██╗  ██╗██╗████████╗
 ██╔══██╗██║██╔════╝██║  ██║██║╚══██╔══╝
 ██████╔╝██║███████╗███████║██║   ██║
 ██╔══██╗██║╚════██║██╔══██║██║   ██║
 ██║  ██║██║███████║██║  ██║██║   ██║
 ╚═╝  ╚═╝╚═╝╚══════╝╚═╝  ╚═╝╚═╝   ╚═╝
```

> *I build systems that don't fall over.*
> *Raft consensus. Sub-50ms inference. Zero data loss on leader failover.*
> *Also: obsessive F1 fan. Mumbai → Tempe.*

[![Portfolio](https://img.shields.io/badge/-rishitbafna.vercel.app-000?style=flat-square&logo=vercel&logoColor=white)](https://rishitbafna.vercel.app)
[![LinkedIn](https://img.shields.io/badge/-rishit--bafna-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/rishit-bafna)
[![Email](https://img.shields.io/badge/-bafnarishit@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:bafnarishit@gmail.com)

</div>

---

<details open>
<summary><b>📡 &nbsp;SIGNAL ACQUIRED — initializing profile...</b></summary>

<br/>

```python
class RishitBafna:
    role       = "Software Engineer"
    degree     = "MS CS @ Arizona State (May 2027)"
    location   = "Tempe, AZ  ·  originally Mumbai, IN"
    interests  = ["distributed systems", "ML pipelines", "Formula 1 🏎️"]
    currently  = "building things at scale · hunting for SWE internships"

    def engineering_philosophy(self):
        return [
            "correctness > performance > developer experience",
            "a well-tested monolith > premature microservices",
            "read the paper, don't just cite it",
        ]

    def fun_facts(self):
        return [
            "I've read the Raft paper more times than is probably healthy",
            "checking lap delta at 2am is a valid use of time",
            "a great system diagram beats 1000 lines of documentation",
            "... but the documentation still ships",
        ]
```

</details>

---

## `> ls -la ./projects`

---

### 🔴 &nbsp;[RiskStream](https://github.com/rbafna1978/riskstream) — real-time fraud detection

```
STATUS      SHIPPED
STACK       Python · XGBoost · FastAPI · PostgreSQL · Redis · MLflow · Docker
HIGHLIGHT   0.96 PR-AUC @ 0.17% class imbalance · p99 < 50ms · zero hot-path DB reads
```

End-to-end ML pipeline over 500K+ transactions. Point-in-time-correct features — no label leakage, training/serving parity verified by tests. PSI-based drift monitoring detects distribution shift and **self-retrains**, hot-swapping the new model without a service restart.

The hard part wasn't the model. It was making sure the features you train on are *exactly* the features you serve — and writing the tests to prove it.

---

### 🟣 &nbsp;[CyberSentient RAG](https://github.com/rbafna1978/cybersentient-rag) — threat intelligence retrieval

```
STATUS      SHIPPED
STACK       Python · Qwen3-Embedding-8B · Qdrant · BM25 · FastAPI
HIGHLIGHT   100K+ CVE/CWE/CAPEC records · 400ms E2E · Qwen3-Reranker-8B
```

Hybrid retrieval: dense vectors + BM25 + Reciprocal Rank Fusion, then cross-encoder reranked to kill false positives on ambiguous CVE lookups. Built for a 6-feed ingestion pipeline over real cybersecurity corpora.

BM25 catches what embeddings miss. Reranking kills what BM25 gets wrong. That's the whole game.

---

### 🟢 &nbsp;[Distributed KV Store](https://github.com/rbafna1978/distributed-kv-store) — Raft from scratch

```
STATUS      SHIPPED
STACK       Java · Raft · gRPC · Protocol Buffers · Docker
HIGHLIGHT   5-node cluster · sub-5ms reads · chaos-tested zero data loss
```

Fault-tolerant key-value store built from first principles — not a tutorial, not a library wrapper. Leader election, log replication, gRPC transport. Chaos-tested: killed nodes mid-write, verified automatic recovery with zero data loss.

Built this because I wanted to *understand* consensus, not just know it exists.

---

### 🔵 &nbsp;[AI Interview Coach](https://interview-helper-three.vercel.app) — voice-driven interview prep

```
STATUS      LIVE
STACK       React · Web Speech API · Node.js · PostgreSQL · OpenAI
DEMO        https://interview-helper-three.vercel.app
```

Browser-native voice transcription — no installs, no setup. Scores answers on STAR structure, filler word density, and pacing in real time. Adaptive difficulty. Session history so you can actually measure improvement.

---

### ⬛ &nbsp;[GitHub Dep Visualizer](https://github.com/rbafna1978/github-dependency-visualizer) — cross-repo dependency graph

```
STATUS      SHIPPED
STACK       React · TypeScript · Node.js · Cytoscape
```

Parses `package.json`, `pom.xml`, `go.mod` across repos into a force-directed graph. Finds the circular deps and version conflicts you didn't know were there.

---

### ⬜ &nbsp;[HTTP Server from Scratch](https://github.com/rbafna1978/http-server) — C++, no frameworks

```
STATUS      SHIPPED
STACK       C++ · Socket Programming · Multithreading
```

Custom thread pool. Raw sockets. Concurrent client handling. The point was to understand what happens between `listen()` and a response — not to ship a product.

---

## `> cat ./experience.log`

```
[Aug 2025 – Dec 2025]  J. Miller Custom Cues  ·  SWE Intern  ·  Tempe, AZ
  → 3D product configurator  (Three.js + React)  — cut revision cycles 35%
  → PostgreSQL REST API + Stripe  — 100+ orders  · sub-200ms response times

[May 2025 – Jul 2025]  Winssoft Technologies  ·  SWE Intern  ·  Mumbai, IN
  → SQL over 200K+ records  — dashboard load: 8s → <2s  (indexes + mat. views)
  → Payment microservice refactor  — 5K+ daily txns  · idempotency guarantees
    eliminated duplicate charge bugs in concurrent request scenarios
```

---

## `> cat ./stack.txt`

| Layer | Tools |
|---|---|
| Languages | Python · Java · TypeScript · JavaScript · C++ · SQL · Go |
| Backend | FastAPI · Node.js · Express · gRPC · WebSockets · REST |
| Frontend | React · Next.js · Three.js · Tailwind CSS |
| Data & ML | PostgreSQL · Redis · Qdrant · XGBoost · PyTorch · MLflow |
| Infra | Docker · AWS (S3, EC2) · Linux · Git |

---

## `> cat ./reading_list.md`

*Papers I've actually read. Not just cited.*

| | Paper | Authors | Year |
|---|---|---|---|
| 📄 | [Raft: In Search of an Understandable Consensus Algorithm](https://raft.github.io/raft.pdf) | Ongaro & Ousterhout | 2014 |
| 📄 | [Dynamo: Amazon's Highly Available Key-value Store](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf) | DeCandia et al. | 2007 |
| 📄 | [Bigtable: A Distributed Storage System for Structured Data](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf) | Chang et al. | 2006 |
| 📄 | [MapReduce: Simplified Data Processing on Large Clusters](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf) | Dean & Ghemawat | 2004 |
| 📄 | [The Google File System](https://static.googleusercontent.com/media/research.google.com/en//archive/gfs-sosp2003.pdf) | Ghemawat, Gobioff & Leung | 2003 |

---

<div align="center">

**MS CS @ ASU &nbsp;·&nbsp; Open to SWE Internships &nbsp;·&nbsp; Backend · Infra · ML Infra**

[bafnarishit@gmail.com](mailto:bafnarishit@gmail.com) &nbsp;·&nbsp; [rishitbafna.vercel.app](https://rishitbafna.vercel.app) &nbsp;·&nbsp; Tempe, AZ

*`// let's build something that doesn't fall over`*

</div>
