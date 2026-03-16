<div align="center">

# Karabo Oliphant

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=1000&color=E2E8F0&center=true&vCenter=true&random=false&width=800&lines=Backend+Engineer+%7C+Distributed+Systems;Storage+Engines+%7C+Job+Queues+%7C+Rate+Limiters;Correctness+under+pressure)](https://git.io/typing-svg)

<p>
  <a href="https://www.linkedin.com/in/karabo-oliphant/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="https://karabootech.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-E2E8F0?style=flat-square&logo=vercel&logoColor=black"/></a>
  <a href="https://github.com/DynamicKarabo"><img src="https://img.shields.io/badge/GitHub-161B22?style=flat-square&logo=github&logoColor=white"/></a>
</p>

<img src="https://komarev.com/ghpvc/?username=DynamicKarabo&label=Profile+Views&color=475569&style=flat-square" />

</div>

---

## About

**What I do** — Backend engineering across distributed systems, storage engines, and infrastructure primitives.
**Where I am** — Junior Software Engineer at **DynamicDNA**, shipping production APIs on a MICT SETA Learnership.
**What I'm building** — A storage engine in C#/.NET implementing WAL, MemTable, and SSTable — studying how databases actually work.

---

## Systems Projects

> Built from first principles.

### Embedded Database Engine
`Python` `B-Tree` `WAL` `Storage Systems`

Bitcask-style append-only storage engine. Write-Ahead Logging with CRC32 checksums for crash-safe durability. In-memory B-Tree index for O(log N) reads and range scans. Background compaction handles tombstone deletion and space reclamation. Covered by **18+ automated tests** across crash recovery and persistence scenarios.

*Taught me how durability guarantees actually work at the byte level — fsync, checksums, and recovery ordering are not details you can abstract away.*

---

### Distributed Job Queue
`Node.js` `TypeScript` `Redis` `Lua` `Express`

Persistent job queue with **at-least-once delivery** via atomic Lua scripts on Redis. Supports priority queuing, delayed execution, exponential backoff, and Dead Letter Queues. DAG-based dependency engine for multi-step task orchestration. Monitoring interface exposes queue depth, job states, and throughput.

*Building this made atomicity concrete — without Lua scripts, race conditions between check-and-act operations are unavoidable.*

---

### Distributed Rate Limiter
`Node.js` `Redis` `Lua` `Prometheus`

Rate limiting infrastructure with atomic Lua execution across **sliding window, cost-based, and multi-window chaining** strategies. Fail-open by design. Full Prometheus observability and containerised CI/CD integration.

*Designing fail-open behaviour forced a real decision: availability vs. strict enforcement — and the answer is context-dependent.*

---

### Distributed Version Control System (Mini Git)
`Python` `SHA-1` `Content-Addressable Storage` `DAG`

Git's object model from scratch — Blobs, Trees, Commits — with SHA-1 content addressing and recursive tree snapshotting. Implements checkout, status, and log. Stress-tested across **130+ automated commits** over hundreds of objects.

*Reimplementing Git clarified why content-addressable storage is elegant: identity and integrity are the same operation.*

---

## Backend Architecture Projects

### Distributed Payment Processing System
`Node.js` `PostgreSQL` `Message Queue`

Idempotent payment processing with duplicate prevention via idempotency keys. Async worker pipeline with exponential backoff and Dead Letter Queues. Transactional integrity enforced at the database layer.

---

### Event-Driven Order Processing Platform
`Node.js` `RabbitMQ` `PostgreSQL`

Microservice architecture over a message broker. Saga-style orchestration for distributed transactions, idempotent consumers, resilient retry strategies, and domain event streams for loose coupling.

---

### API Gateway with Distributed Rate Limiting
`Node.js` `Redis` `Prometheus`

API gateway handling routing, authentication, and rate limiting. Lua-based Redis rate limiter in the middleware chain alongside auth, logging, and traffic shaping. Prometheus instrumentation with latency histograms.

---

## Tech Stack

```
Languages       Python · TypeScript · JavaScript · C#
Backend         Node.js · FastAPI · .NET Web API · REST APIs
Data & Storage  PostgreSQL · Redis · Message Queues · Storage Engines
Infrastructure  Docker · Linux · Prometheus
Tools           Git · GitHub
```

---

## Experience

**Junior Software Engineer — DynamicDNA** *(Sep 2025 – Present)*
Building backend APIs in Node.js and TypeScript across corporate, education, and non-profit platforms. Responsible for authentication systems, data persistence layers, third-party service integrations, and deployment pipeline maintenance across multiple production environments.

---

## Education

| | |
|---|---|
| **Level 4 System Development** | DynamicDNA · MICT SETA Learnership · 2025–Present |
| **Software Engineering** | ALX Africa · Feb–Aug 2024 |

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=DynamicKarabo&show_icons=true&theme=dark&hide_border=true&bg_color=0D1117&title_color=E2E8F0&icon_color=475569&text_color=94A3B8" width="47%" />
<img src="https://github-readme-streak-stats.herokuapp.com/?user=DynamicKarabo&theme=dark&hide_border=true&background=0D1117&ring=475569&fire=E2E8F0&currStreakLabel=E2E8F0" width="47%" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=DynamicKarabo&layout=compact&theme=dark&hide_border=true&bg_color=0D1117&title_color=E2E8F0&text_color=94A3B8&langs_count=6" width="40%" />

</div>

---

<div align="center">

`karabooliphant34@gmail.com` · Johannesburg, South Africa

*The systems speak for themselves.*

</div>
