# Rishit Bafna

**MS Computer Science @ Arizona State University**  
**Building distributed systems and shipping production software**

I build systems that handle real scale. Recently shipped a [production 3D configurator](https://jmillercustomcues.com) serving live customers with Stripe payments. Currently implementing Raft consensus and CRDT-based collaborative editing from scratch.

---

## 🚀 What I'm Building

### [Distributed Key-Value Store](https://github.com/rbafna1978/distributed-kv-store) ⭐
Fault-tolerant database implementing **Raft consensus algorithm** in Java with gRPC.

**Key features:**
- Leader election & log replication across 5-node cluster
- Automatic failover during network partitions
- 45K writes/sec, sub-5ms P99 latency (JMeter tested with 10K concurrent clients)

**Tech:** Java • Raft • gRPC • Protobuf • JMeter

---

### [Real-Time Collaborative Code Editor](https://github.com/rbafna1978/collaborative-editor) ⭐
Multi-user code editor using **Conflict-free Replicated Data Types (CRDT)** for operational transformation.

**Key features:**
- 50+ simultaneous users per document with eventual consistency
- WebSocket server with Redis pub/sub for horizontal scaling
- 1000+ concurrent connections with automatic reconnection

**Tech:** React • WebSockets • CRDT • Redis • Docker

---

### [C Compiler with LLVM Backend](https://github.com/rbafna1978/c-compiler)
Complete compiler with lexer, parser, semantic analysis, and **LLVM IR code generation**.

**Key features:**
- Supports functions, structs, pointers, arrays, control flow
- SSA-based optimizations: constant folding, dead code elimination, register allocation
- 15% runtime improvement over unoptimized baseline

**Tech:** C++ • LLVM • Flex/Bison • SSA

---

### [Multithreaded HTTP Server](https://github.com/rbafna1978/http-server)
HTTP/1.1 web server from scratch in C++ using POSIX sockets.

**Key features:**
- Thread pool with work-stealing queue
- 1000+ concurrent connections, 25K req/sec throughput (ApacheBench)
- Lock-free request parsing

**Tech:** C++ • POSIX • TCP Sockets • Multithreading

---

## 💼 Shipped to Production

**3D Product Configurator @ J. Miller Custom Cues** (Aug - Dec 2025)  
Built and shipped full-stack configurator **currently live** on company website processing real customer orders.

- Three.js + React for real-time 3D rendering with WebGL
- PostgreSQL REST API with Stripe payment integration
- Reduced customer design revisions by 35%
- Sub-200ms API response times in production

**[See it live →](https://jmillercustomcues.com)**

---

## 🛠️ Tech Stack

**Systems:** Java • C++ • C • Distributed Systems • Raft • CRDT  
**Backend:** Node.js • FastAPI • gRPC • WebSockets • REST  
**Databases:** PostgreSQL • Redis • MongoDB • MySQL  
**Tools:** Docker • Linux • Git • AWS • JMeter • LLVM • ApacheBench

---

## 📫 Connect

- **Email:** bafnarishit@gmail.com
- **LinkedIn:** [linkedin.com/in/rishit-bafna](https://linkedin.com/in/rishit-bafna)
- **Resume:** [View PDF](https://drive.google.com/file/d/1CGEiqjPd6OnAdfhIHydKLFlb8wsbA0Z8/view?usp=sharing)

---

**Currently:** Building production-ready distributed systems • MS in CS @ ASU (Expected May 2027)
