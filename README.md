<div align="center">

# Karabo Oliphant

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=1000&color=E2E8F0&center=true&vCenter=true&random=false&width=800&lines=Backend+Engineer+%7C+C%23%2F.NET+Specialist;Payments+%7C+Reconciliation+%7C+Financial+Compliance;Multi-tenant+Architectures+%7C+Auditability)](https://git.io/typing-svg)

<p>
  <a href="https://www.linkedin.com/in/karabo-oliphant/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="https://karabootech.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-E2E8F0?style=flat-square&logo=vercel&logoColor=black"/></a>
  <a href="https://github.com/DynamicKarabo"><img src="https://img.shields.io/badge/GitHub-161B22?style=flat-square&logo=github&logoColor=white"/></a>
</p>

<img src="https://komarev.com/ghpvc/?username=DynamicKarabo&label=Profile+Views&color=475569&style=flat-square" />

</div>

---

## About

**What I do** — Backend engineering with C#/.NET, specializing in payments, reconciliation, and financial compliance systems.

**Where I am** — Junior Software Engineer at **DynamicDNA**, building production APIs on a MICT SETA Learnership. Previously at **LendFlow** (micro-lending credit API) and **PayFlow** (multi-tenant payment platform).

**What I'm building** — Financial infrastructure primitives: idempotent payment flows, reconciliation engines, and audit-compliant transaction processing.


---

## Selected Projects

> Built from first principles.

### Financial Reconciliation Engine
`C#` `.NET 8` `SQL Server` `Redis`

Multi-step matching pipeline: exact → fuzzy (Jaro-Winkler) → configurable rule-based matching. Idempotent ingestion on (Source, ExternalId) to prevent duplicate records. Append-only audit log for traceability and compliance. POPIA-conscious design with encrypted fields and Azure Key Vault key management.

*Reconciliation taught me that matching logic must be explicit and auditable — every decision needs a trace.*

---

### KYC / FICA Onboarding Service
`C#` `.NET 8` `SQL Server` `Azure Blob Storage` `Hangfire`

Customer onboarding aligned with South African FICA compliance. SA ID validation with Luhn check and structural validation. Risk scoring combining PEP flags, sanctions checks, and document quality. State machine with enforced, auditable transitions. Secure document handling via Azure Blob Storage with SAS tokens.

*Compliance isn't a checkbox — it's a state machine with enforced transitions.*

---

### Database Migration CLI Tool
`C#` `.NET 8` `SQL Server`

Versioned SQL migrations with checksum validation and safe concurrent execution. Supports rollback detection and migration status tracking.

---

### Field Service Management Platform
`C#` `.NET 8` `SignalR` `SQL Server`

Job dispatching with SLA tracking and real-time updates using SignalR. Multi-tenant architecture with tenant isolation.

---

### Distributed Job Queue
`Node.js` `TypeScript` `Redis` `Lua` `Express`

Persistent job queue with **at-least-once delivery** via atomic Lua scripts on Redis. Supports priority queuing, delayed execution, exponential backoff, and Dead Letter Queues. DAG-based dependency engine for multi-step task orchestration.

---

### Storage Engine (Learning Project)
`C#` `.NET 8` `B-Tree` `WAL`

Bitcask-style append-only storage engine. Write-Ahead Logging with CRC32 checksums for crash-safe durability. In-memory B-Tree index for O(log N) reads. Background compaction handles tombstone deletion.

---

### Event Aggregation Pipeline
`C#` `.NET 8` `SQL Server`

Precomputed time-series metrics with support for late-arriving events. Background aggregation jobs with configurable windows and incremental updates.

---

## Tech Stack

```
Languages       C# · TypeScript · JavaScript · Python
Backend         .NET 8 · ASP.NET Core · Node.js · REST APIs
Data & Storage  SQL Server · Redis · Entity Framework Core · Dapper
Infrastructure  Azure Service Bus · Azure Blob Storage · Azure Key Vault · Docker
Patterns        Clean Architecture · CQRS · MediatR · State Machines
Observability   OpenTelemetry · Prometheus · Hangfire
Tools           Git · GitHub
```

---

## Experience

**DynamicDNA — MICT SETA Learnership, Level 4** *(Sep 2025 – Present)*
Building backend APIs across corporate, education, and non-profit platforms. Contributing to client-facing applications, deployment pipelines, and system design discussions.

---

### LendFlow — Micro-Lending Credit Application API
*Built as part of DynamicDNA learnership*

Multi-tenant backend API for the full micro-loan lifecycle (application, decisioning, disbursement, repayment). Tenant isolation via EF Core query filters. Explicit state machines for loan applications with validated transitions. Idempotent disbursements using Redis to prevent double payments. POPIA-aware PII handling with encryption at rest. Append-only audit logging for traceable state transitions.

---

### PayFlow — Multi-Tenant Payment Processing Platform
*Built as part of DynamicDNA learnership*

Multi-tenant payment processing with tenant scoping via EF Core query filters. Idempotent payment handling using Redis SET NX to prevent duplicate charges. Payment state model (Created → Authorised → Captured → Settled) enforced at domain layer. Webhook delivery with exponential backoff and HMAC-SHA256 signed payloads. Partial refunds and settlement batching.

---

## Education

| | |
|---|---|
| **Level 4 System Development** | DynamicDNA · MICT SETA Learnership · 2025–Present |
| **Software Engineering** | ALX Africa · Feb–Aug 2024 |

---

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=DynamicKarabo&show_icons=true&theme=dark&hide_border=true&bg_color=0D1117&title_color=E2E8F0&icon_color=475569&text_color=94A3B8)](https://github.com/DynamicKarabo)
[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=DynamicKarabo&theme=dark&hide_border=true&background=0D1117&ring=475569&fire=E2E8F0&currStreakLabel=E2E8F0)](https://github.com/DynamicKarabo)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=DynamicKarabo&layout=compact&theme=dark&hide_border=true&bg_color=0D1117&title_color=E2E8F0&text_color=94A3B8&langs_count=6)](https://github.com/DynamicKarabo)

</div>

---

<div align="center">

`karabooliphant34@gmail.com` · Johannesburg, South Africa

*The systems speak for themselves.*

</div>
