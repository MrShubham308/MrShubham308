# ⚡ Hello World, I'm Shubham Vishwakarma 👋

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=3000&pause=1000&color=7aa2f7&center=true&vCenter=true&width=700&lines=Staff+Software+Engineer;Distributed+Systems+%7C+Cloud+Native+%7C+AI+Infra;Building+Resilient%2C+Hyper-Scale+Architectures" alt="Typing SVG" />
</p>
<p align="center">
  <a href="https://linkedin.com" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:itzshubham81@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

  <a href="https://shubhamvihswakarma.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-101010?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"/></a>
  <a href="https://leetcode.com/u/mrshubham06/"><img src="https://img.shields.io/badge/-LeetCode-FFA116?style=for-the-badge&logo=LeetCode&logoColor=black" alt="LeetCode"/></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=alexchen-dev&color=7aa2f7&style=flat-square&label=PROFILE+VIEWS" alt="Visitor Counter"/>
  <img src="https://img.shields.io/github/followers/alexchen-dev?label=Followers&style=flat-square&color=bb9af7" alt="Followers"/>
</p>

---

## 🚀 About Me

I am a **Staff Software Engineer** specializing in **Distributed Systems, Cloud-Native Architectures, and AI Infrastructure**. My engineering philosophy centers on building deterministic, fault-tolerant systems that operate seamlessly at hyper-scale. Driven by mechanical sympathy and rigorous systems design, I bridge the gap between complex research and production-grade reliability.

*   🎓 **Education:**deen dayal upadhyaya gorakhpur university Gorakhpur
*   🎯 **Career Goals:** Architecting the next generation of real-time multi-agent AI execution layers and ultra-low latency state stores.
*   🧠 **Specialization:** High-throughput event-driven microservices, consensus protocols (Raft/Paxos), consensus-backed caching, and high-performance Rust core modules.

---

## 🏆 Competitive Programming & Achievements

*   💡 **LeetCode:** Guardian Rank (Top 0.5%, Max Rating: 2450+, 1200+ Problems Solved)
*   🏅 **Codeforces:** Master (Max Rating: 2100+)
*   🏆 **Hackathons:** 1st Place Winner out of 500+ teams at Global Web3 & AI Infra Hackathon (2025)
*   📜 **Certifications:** AWS Certified Solutions Architect – Professional • Certified Kubernetes Administrator (CKA)
*   🎖️ **Academic Excellence:** Graduated Summa Cum Laude, Outstanding Research Thesis Award in Distributed Consensus.

---

## 💼 Featured Projects

### 🌟 Project 1: NexaStore — Ultra-Low Latency Distributed Key-Value Store
> **Core Architecture:** Rust • Raft Consensus • gRPC • eBPF • RocksDB Storage Engine

*   **Business Problem:** Legacy state management layers introduced unacceptable tail latencies ($p99.9 > 150\text{ms}$) during flash-sale traffic spikes, causing cascading timeouts in downstream checkouts.
*   **System Architecture:** A distributed, sharded LSM-tree structured data store utilizing a custom optimized Raft consensus implementation over zero-copy gRPC transport layers.
*   **Scalability & Performance:** Achieved horizontal write-scalability by employing consistent hashing with bounded loads. Handles **1.2M+ RPS** with $p99$ latency tightly bounded at **$1.8\text{ms}$**.
*   **Security Stack:** TLS 1.3 mutual authentication (mTLS) for all inter-node RPCs, hardware-accelerated AES-256-GCM encryption-at-rest via Intel AES-NI instructions, and fine-grained RBAC.
*   **Engineering Challenge:** Resolving unpredictable tail-latency spikes caused by stop-the-world garbage collection and disk I/O serialization during concurrent Raft log compactions. 
*   **Production Implementation:** Rewrote the compaction pipeline utilizing thread-per-core architecture via the Tokio runtime, bypassing the OS page cache using direct I/O (`O_DIRECT`), and leveraging eBPF for accelerated network packet routing directly to the target shard driver.

### 🌟 Project 2: AetherFlow — Real-Time Event-Driven Telemetry Engine
> **Core Architecture:** Go • Apache Kafka • Kubernetes • ClickHouse • Redis Cluster

*   **Business Problem:** Fragmented streaming architecture was incapable of processing high-velocity IoT and application telemetry data simultaneously, leading to delayed anomaly detection and data loss.
*   **System Architecture:** Multi-tier decoupled ingestion pipeline leveraging partition-balanced Kafka brokers, highly parallel Go-based consumer groups with lock-free ring buffers, and a columnar ClickHouse analytical store.
*   **Scalability & Performance:** Horizontally scalable ingestion layer processing over **50 Terabytes** of streaming telemetry daily, maintaining linear scalability up to **200 Nodes** via Kubernetes HPA.
*   **Security Stack:** End-to-end payload signature verification using HMAC-SHA256, isolated VPC network topologies, and automated secret rotations handled via HashiCorp Vault.
*   **Engineering Challenge:** Managing extreme out-of-order data event delivery and deduplication logic across highly unstable network topologies without bottlenecking database write throughput.
*   **Production Implementation:** Implemented a hybrid sliding-window time-bucket algorithm in Go using atomic memory operations. Utilized ClickHouse `ReplacingMergeTree` engine to guarantee idempotency and perform asynchronous background deduplication, sustaining database write speeds of **800k rows/sec**.

---

## ⚡ Engineering Stack

| Layer | Technologies |
| :--- | :--- |
| **💻 Programming Languages** | `Rust` `Go` `C++` `Python` `TypeScript` `Java` `SQL` |
| **🎨 Frontend Development** | `Next.js` `React` `TypeScript` `TailwindCSS` `WebAssembly` `GraphQL` |
| **⚙️ Backend Engineering** | `Node.js` `Gin` `Axum` `Tokio` `Spring Boot` `gRPC` `Protocol Buffers` |
| **🗄️ Databases** | `PostgreSQL` `ClickHouse` `Redis` `MongoDB` `RocksDB` `Cassandra` |
| **☁️ Cloud & DevOps** | `AWS` `Kubernetes` `Docker` `Terraform` `GitHub Actions` `Prometheus` `Grafana` |
| **🤖 Artificial Intelligence** | `PyTorch` `LangChain` `LlamaIndex` `HuggingFace` `vLLM` `Milvus` |
| **📊 Data Engineering** | `Apache Kafka` `Apache Spark` `Flink` `Airflow` `Snowflake` |
| **🔐 Security & Infrastructure** | `eBPF` `HashiCorp Vault` `OAuth2/OIDC` `mTLS` `WireGuard` |

---

## 🏗️ Engineering Experience
