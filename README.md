<div align="center">

# Karabo Oliphant

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=1000&color=E2E8F0&center=true&vCenter=true&random=false&width=800&lines=Backend+Engineer+%7C+Distributed+Systems;Storage+Engines+%7C+Job+Queues+%7C+Rate+Limiters;Building+reliable+infrastructure+from+scratch)](https://git.io/typing-svg)

<p>
  <a href="https://www.linkedin.com/in/karabo-oliphant/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="https://karabootech.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-E2E8F0?style=flat-square&logo=vercel&logoColor=black"/></a>
  <a href="https://github.com/DynamicKarabo"><img src="https://img.shields.io/badge/GitHub-161B22?style=flat-square&logo=github&logoColor=white"/></a>
</p>

<img src="https://komarev.com/ghpvc/?username=DynamicKarabo&label=Profile+Views&color=475569&style=flat-square" />

</div>

---

## About

Backend engineer focused on **distributed systems, storage engines, and infrastructure**. I build things that are fault-tolerant, observable, and correct under pressure — write-ahead logs, atomic job queues, DAG-based orchestration, and distributed rate limiters.

Currently a Junior Software Engineer at **DynamicDNA** (MICT SETA Learnership), building production APIs across corporate, education, and non-profit platforms.

---

## Systems Projects

> The work I'm most proud of — systems built from first principles.

### 🗄️ Embedded Database Engine
`Python` `B-Tree` `WAL` `Storage Systems`

Bitcask-style append-only storage engine with Write-Ahead Logging and CRC32 checksums for crash-safe durability. In-memory B-Tree index for O(log N) lookups and range scanning. Background compaction and tombstone deletion for space reclamation. Verified with **18+ automated tests** covering crash recovery and persistence.

---

### ⚙️ Distributed Job Queue
`Node.js` `TypeScript` `Redis` `Lua` `Express`

Distributed job queue with persistent storage and **at-least-once delivery guarantees** using Redis and atomic Lua scripts. Priority queuing, delayed execution, exponential backoff retry, and Dead Letter Queues. DAG-based dependency engine for complex task orchestration with a monitoring interface exposing queue metrics and job state transitions.

---

### 🚦 Distributed Rate Limiter
`Node.js` `Redis` `Lua` `Prometheus`

Infrastructure-grade rate limiter with atomic Lua execution supporting **sliding window, cost-based, and multi-window chaining** algorithms. Fail-open reliability, Prometheus metrics observability, and containerised CI/CD workflows.

---

### 🔀 Distributed Version Control System (Mini Git)
`Python` `SHA-1` `Content-Addressable Storage` `DAG`

Git's core object model reimplemented from scratch — Blobs, Trees, Commits — with SHA-1 hashing and recursive tree snapshotting. Built checkout, status, and log commands. Stress-tested with **130+ automated commits** across hundreds of objects.

---

## Backend Architecture Projects

### 💳 Distributed Payment Processing System
`Node.js` `PostgreSQL` `Message Queue`

Idempotent payment processing preventing duplicate transactions. Async processing via message queues and worker services, exponential backoff retry with Dead Letter Queues, transactional integrity through database constraints and idempotency keys.

---

### 📦 Event-Driven Order Processing Platform
`Node.js` `RabbitMQ` `PostgreSQL`

Microservices communicating through a message broker. Saga-style orchestration for distributed transactions, idempotent event handling, resilient consumers with retry strategies, and loose coupling through domain event streams.

---

### 🔀 API Gateway with Distributed Rate Limiting
`Node.js` `Redis` `Prometheus`

High-performance API gateway handling request routing, authentication, and rate limiting. Atomic Lua-based Redis rate limiter integrated into a middleware pipeline supporting auth, logging, and traffic shaping. Prometheus metrics with latency histograms.

---

## Tech Stack

```
Languages       Python · TypeScript · JavaScript
Backend         Node.js · FastAPI · .NET Web API · REST APIs
Data & Storage  PostgreSQL · Redis · Message Queues · Storage Engines
Infrastructure  Docker · Linux · Prometheus
Tools           Git · GitHub
```

---

## Experience

**Junior Software Engineer — DynamicDNA** *(Sep 2025 – Present)*
Backend APIs in Node.js and TypeScript. Authentication, data persistence, external integrations, deployment pipelines.

---

## Education

| | |
|---|---|
| **Level 4 System Development** | DynamicDNA · MICT SETA Learnership · 2025–Present |
| **Software Engineering** | ALX Africa · Feb–Aug 2024 |

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=DynamicKarabo&show_icons=true&theme=dark&hide_border=true&bg_color=0D1117&title_color=E2E8F0&icon_color=475569&text_color=94A3B8" width="48%" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=DynamicKarabo&theme=dark&hide_border=true&background=0D1117&ring=475569&fire=E2E8F0&currStreakLabel=E2E8F0" width="48%" />

</div>

---

<div align="center">

`karabooliphant34@gmail.com` · Johannesburg, South Africa

*Building reliable systems, one abstraction at a time.*

</div>
