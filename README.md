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

**What I do** — Backend engineering with C#/.NET, specializing in payments, reconciliation, and financial compliance (FICA/POPIA). Experienced designing multi-tenant architectures built for correctness, auditability, and graceful failure handling. Comfortable across messaging systems, background processing, and distributed workflows.

**Where I am** — Enrolled in a **MICT SETA Level 4 System Development Learnership** at **DynamicDNA**. Contributing to client-facing applications across corporate, education, and non-profit platforms. Built **LendFlow** (micro-lending credit API) and **PayFlow** (multi-tenant payment platform) as learnership projects.

**What I'm building** — Financial infrastructure primitives: idempotent payment flows, reconciliation engines, and audit-compliant transaction processing.

---

## Selected Projects

> Built from first principles.

### LendFlow — Micro-Lending Credit Application API
`C#` `.NET 8` `ASP.NET Core` `SQL Server` `Redis` `Azure Service Bus` `Hangfire` `EF Core` `Dapper`

Multi-tenant backend API for the full micro-loan lifecycle (application → decisioning → disbursement → repayment), with auditability and compliance as first-class concerns.

- Tenant isolation via global EF Core query filters and TenantId on all entities.
- Explicit state machines for loan applications with validated transitions.
- Idempotent financial operations using Redis keys to prevent double disbursements.
- POPIA-aware PII handling with encryption at rest and minimal data exposure.
- Append-only audit logging for traceable state transitions and regulatory reporting.

---

### PayFlow — Multi-Tenant Payment Processing Platform
`C#` `.NET 8` `SQL Server` `Redis` `Azure Service Bus` `Hangfire` `Docker`

Payment processing system focused on safe retries, tenant isolation, and traceable payment flows.

- Tenant scoping with EF Core query filters to eliminate cross-tenant data access risk.
- Idempotent payment handling using Redis SET NX to prevent duplicate charges on retries.
- Payment state model (Created → Authorised → Captured → Settled) enforced at domain layer.
- Webhook delivery system with exponential backoff retries and HMAC-SHA256 signed payloads.
- Partial refunds, settlement batching, and test/live environment separation.

---

### Financial Reconciliation Engine
`C#` `.NET 8` `SQL Server` `Azure Service Bus` `MediatR` `Hangfire`

Transaction matching system to reconcile records across multiple financial sources.

- Multi-step matching pipeline: exact → fuzzy (Jaro-Winkler) → configurable rule-based matching.
- Idempotent ingestion on (Source, ExternalId) to prevent duplicate records.
- Append-only audit log for traceability and compliance requirements.
- Exception workflow with categorisation (mismatch, duplicate) and manual review support.
- POPIA-conscious design: minimal PII, encrypted fields, keys managed via Azure Key Vault.

*Reconciliation taught me that matching logic must be explicit and auditable — every decision needs a trace.*

---

### KYC / FICA Onboarding Service
`C#` `.NET 8` `SQL Server` `Azure Blob Storage` `Hangfire` `Key Vault`

Customer onboarding system aligned with South African FICA compliance requirements.

- SA ID validation logic including Luhn check and full structural validation.
- Risk scoring system combining PEP flags, sanctions checks, and document quality signals.
- Onboarding flow modelled as a state machine with enforced, auditable transitions.
- Secure document handling via Azure Blob Storage private access and SAS tokens.
- Role-based workflows for enhanced due diligence and multi-level approvals.

*Compliance isn't a checkbox — it's a state machine with enforced transitions.*

---

## Additional Projects

**Event Sourcing & CQRS Reference Implementation** — Append-only event store with aggregate replay, transactional outbox, and optimistic concurrency on PostgreSQL.

**Real-Time Notification Engine** — SignalR hub with Redis backplane, presence tracking, and exactly-once event delivery via Redis Streams.

**EquiLink** — Production-grade institutional trading platform designed for asset managers, hedge funds, and prop trading firms.

---

## Tech Stack

```
Backend         C# · .NET 8 · ASP.NET Core · Entity Framework Core · MediatR
Data            SQL Server · Redis
Infrastructure  Azure Service Bus · Azure Blob Storage · Azure Key Vault · Docker · Linux
Patterns        Clean Architecture · CQRS · State Machines · Event-driven Systems
Observability   OpenTelemetry · Prometheus
Other           TypeScript · JavaScript · Python · Node.js
```

---

## Experience

**DynamicDNA — MICT SETA Learnership, Level 4** *(Sep 2025 – Present)*
Contributing to client-facing web applications across corporate, education, and non-profit sectors. Participating in deployment processes and collaborating on system design discussions. Building supporting backend components and improving reliability of existing features.

---

## Education

| | |
|---|---|
| **Level 4 System Development** | MICT SETA · System Development Learnership |
| **Software Engineering** | ALX Africa · Software Engineering Programme |

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
