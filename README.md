# hey, i'm rishit 👋

MS CS @ Arizona State · building things that don't fall over

I care about backend systems and ML that actually works in production — not notebooks, not demos, not wrappers around an API. If it doesn't have latency targets, drift monitoring, and a way to fail gracefully, it's not done.

When I'm not writing code I'm watching F1 or arguing about NBA advanced stats — turns out both are just distributed systems with worse uptime.

---

## three things I'd bring up in an interview before you asked

**A "hard on tires" driver rating was actually just a fast car.** Building the F1 strategy model, I scored each driver's tire management as the slope of lap time vs. tire age. The number looked clean — until I noticed it was quietly rating every driver in a fast car as "hard on tires," because a fast car degrades its tires visibly regardless of driving style. Fixed it by comparing each driver only to their own teammate in the same race — identical machinery, isolates the human variable. Perez and Bottas flipped from "hard" to correctly "easy" the moment I did.

**A model that scored worse than a coin flip taught me to check my labels before my architecture.** The DNF-risk sub-model started at AUC 0.35 — actively anti-predictive. The bug wasn't the model, it was upstream: I'd labeled DNFs from a free-text status string instead of Ergast's structured finish-position field, which silently mislabeled cars that finished laps down as retirements. Fixing the label alone took it from 0.35 to 0.645; a driver-form embedding pushed it to 0.70.

**An anomaly score is a feature, not a verdict.** RiskStream's fraud detector doesn't hard-gate on the Isolation Forest anomaly score — it feeds that score into XGBoost as a 14th input and lets the model learn how much to trust it. A hard gate turns every false anomaly into a false decline; letting XGBoost weigh it against thirteen other features cut false positives without cutting recall.

---

## what i've built

[#what-ive-built](#what-ive-built)

**[F1 Race Strategy RL](https://github.com/rbafna1978/f1_strategy)** — PPO agent for real F1 race strategy
Multi-agent environment covering all 20 cars, 142-dimensional observation space, counterfactual reward shaping, learned driver/constructor form embeddings. 188K laps of historical data (2018–2025), with three frozen sub-models (tire degradation, DNF risk, safety-car probability) acting as a physics engine under the RL layer. Started after reading Imperial/Mercedes' RSRL paper and thinking the multi-agent version was worth building.

`Python · PyTorch · FastAPI · React · OpenF1`

---

**[RiskStream](https://github.com/rbafna1978/RiskStream)** — end-to-end fraud detection over 500K transactions
Point-in-time correct features (no label leakage), XGBoost + Isolation Forest, PR-AUC 0.96 at 0.17% class imbalance. FastAPI inference at p99 < 50ms with zero hot-path DB reads. PSI-based drift monitoring retrains and hot-swaps the model without a service restart. Built because most fraud-detection tutorials stop before the part that matters.

`Python · XGBoost · FastAPI · Redis · MLflow · Docker · PostgreSQL`

---

**CyberSentient RAG** *(private team repo)* — hybrid retrieval over 100K+ CVE/CWE/CAPEC records
Dense vectors + BM25 + Reciprocal Rank Fusion, cross-encoder reranked to kill false positives on ambiguous CVE lookups. 400ms end-to-end across a 6-feed ingestion pipeline. My piece was the hybrid retrieval pipeline and the writeup.

`Python · Qwen3-Embedding-8B · Qdrant · BM25 · FastAPI`

---

**[Distributed KV Store](https://github.com/rbafna1978/distributed-kv-store)** — Raft consensus from scratch
5-node cluster, gRPC transport, sub-5ms reads, chaos-tested leader failover with zero data loss. Built this to actually understand the protocol, not just cite the paper.

`Java · Raft · gRPC · Protocol Buffers · Docker`

---

**[AI Interview Coach](https://interview-helper-three.vercel.app)** — live voice transcription, real-time feedback · [live ↗](https://interview-helper-three.vercel.app)
Browser-native voice via Web Speech API. Scores STAR structure, filler word density, and pacing in under 3 seconds. Used by 50+ students.

`React · Web Speech API · Node.js · PostgreSQL`

---

## papers i've read and actually used

[#papers-ive-read-and-actually-used](#papers-ive-read-and-actually-used)

- [Raft: In Search of an Understandable Consensus Algorithm](https://raft.github.io/raft.pdf) — built a 5-node cluster from it
- [Explainable RL for F1 Race Strategy](https://arxiv.org/abs/2501.04068) — Mercedes/Imperial, SAC'25 — sparked the F1 RL project, borrowed the tire allocation insight
- [Dynamo: Amazon's Highly Available Key-Value Store](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf)
- [Bigtable: A Distributed Storage System for Structured Data](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf)
- [The Google File System](https://static.googleusercontent.com/media/research.google.com/en//archive/gfs-sosp2003.pdf)
- [MapReduce: Simplified Data Processing on Large Clusters](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)

---

## stack

[#stack](#stack)

```
languages    Python  Java  TypeScript  JavaScript  C++  SQL
backend      FastAPI  Node.js  Express  gRPC  WebSockets
ml / data    XGBoost  PyTorch  scikit-learn  MLflow  Qdrant  Redis
frontend     React  Next.js  Three.js  Tailwind
infra        Docker  AWS (S3, EC2)  PostgreSQL  Linux
```

---

## where i've shipped production code

[#where-ive-shipped-production-code](#where-ive-shipped-production-code)

**J. Miller Custom Cues** (Aug–Dec 2025) — 3D product configurator in Three.js + React, cut revision cycles 35%. PostgreSQL REST API + Stripe, 100+ orders, sub-200ms.

**Winssoft Technologies** (May–Jul 2025) — optimized SQL over 200K+ records, 8s → 2s. Refactored payment microservice with idempotency guarantees across 5K+ daily transactions.

---

open to new grad SWE roles · backend · ML infra · distributed systems · Tempe, AZ

<bafnarishit@gmail.com> · [linkedin](https://linkedin.com/in/rishit-bafna) · [portfolio](https://rishitbafna.vercel.app)
