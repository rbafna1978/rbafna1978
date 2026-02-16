# Rishit Bafna

  MS Computer Science @ Arizona State University (May 2027)
  Building distributed systems and shipping production software


I build systems that handle real scale. Recently shipped a [production 3D configurator](https://jmillercustomcues.com) serving live customers. Currently implementing Raft consensus and high-performance full-stack tools.

  ---

  🚀 What I'm Building


  [Distributed Key-Value Store](https://github.com/rbafna1978/distributed-kv-store) ⭐
  Fault-tolerant database implementing Raft consensus algorithm in Java with gRPC.


   - Leader election & log replication across 5-node cluster
   - Automatic failover during network partitions
   - 45K writes/sec, sub-5ms P99 latency (JMeter tested with 10K concurrent clients)

  Tech: Java • Raft • gRPC • Protobuf • JMeter

  ---


  [Interview Coach AI](https://github.com/rbafna1978/Interview_Helper) ⭐
  Full-stack behavioral & technical interview prep platform with local-first AI scoring.


   - Optimized architecture by migrating from a legacy Python transcription service to browser-native Web Speech API for zero-latency, local-first processing.
   - Built a custom TypeScript scoring engine evaluating STAR method structure, delivery metrics (WPM, fillers), and technical relevance.
   - Secure, passwordless authentication using NextAuth OTP and session-claiming for guest history.

  Tech: Next.js 16 • React 19 • PostgreSQL • Prisma • Web Speech API

  ---


  [C Compiler with LLVM Backend](https://github.com/rbafna1978/c-compiler)
  Complete compiler with lexer, parser, semantic analysis, and LLVM IR code generation.


   - Supports functions, structs, pointers, arrays, and control flow
   - SSA-based optimizations: constant folding, dead code elimination, and register allocation
   - 15% runtime improvement over unoptimized baseline

  Tech: C++ • LLVM • Flex/Bison • SSA

  ---


  [Multithreaded HTTP Server](https://github.com/rbafna1978/http-server)
  HTTP/1.1 web server from scratch in C++ using POSIX sockets.

   - Thread pool with work-stealing queue for efficient task distribution
   - Handles 1000+ concurrent connections, 25K req/sec throughput
   - Lock-free request parsing for minimal overhead


  Tech: C++ • POSIX • TCP Sockets • Multithreading

  ---

  💼 Shipped to Production


  3D Product Configurator @ J. Miller Custom Cues (Aug - Dec 2025)
  Built and shipped a full-stack configurator currently live processing real customer orders.

   - Three.js + React for real-time 3D rendering with WebGL
   - PostgreSQL REST API with Stripe payment integration
   - Reduced customer design revisions by 35%
   - Sub-200ms API response times in production


  [See it live →](https://jmillercustomcues.com)

  ---

  🛠️ Tech Stack


  Systems: Java • C++ • C • Distributed Systems • Raft • LLVM • POSIX
  Backend: Node.js • Next.js • FastAPI • gRPC • WebSockets • REST
  Databases: PostgreSQL • Redis • MongoDB • MySQL • Prisma
  Tools: Docker • Linux • Git • AWS • JMeter • ApacheBench

  ---

  📫 Connect


   - [Email](mailto:bafnarishit@gmail.com)
   - [LinkedIn](https://linkedin.com/in/rishit-bafna)
   - [Portfolio](https://rishitbafna.vercel.app)

  ---


  Currently: Building production-ready distributed systems • MS in CS @ ASU (Expected May 2027)
