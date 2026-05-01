<div align="center">

# **Karabo Oliphant**
### Backend Engineer · Johannesburg, South Africa 🇿🇦

[![GitHub followers](https://img.shields.io/github/followers/DynamicKarabo?style=for-the-badge&logo=github&color=0e75b6)](https://github.com/DynamicKarabo)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/karabo-oliphant)
[![Email](https://img.shields.io/badge/Email-Reach%20Out-red?style=for-the-badge&logo=gmail)](mailto:karabo.oliphant34@gmail.com)

</div>

---

> **I build production backends.** .NET is my core. Distributed systems, transactional integrity, and infrastructure that survives production. From payment processing to fraud detection to lending platforms — systems that handle real money without falling over.

---

## Backend Systems

| Project | Stack | Architecture |
|---------|-------|-------------|
| **LendFlow** | `.NET 10` `SQL Server` `Redis` `Azure Service Bus` | Multi-tenant micro-lending platform. Tenant isolation, idempotent loan lifecycle, POPIA-compliant PII handling. State machine-driven application processing. |
| **PayFlow** | `.NET 9` `SQL Server` `Redis` `Hangfire` | Payment processing with enforced state machine (Initiated→Authorised→Captured→Settled). Idempotent retries, HMAC-SHA256 webhooks, merchant reconciliation. |
| **EquiLink** | `.NET 8` `PostgreSQL` `Redis` | Institutional trading middleware on CQRS + append-only event sourcing. Pre-trade risk engine via chain-of-responsibility. WORM archival for 7-year regulatory compliance. |
| **RT-FDE** | `.NET 8` `Redis` `SQL Server` | Real-time fraud scoring at the Authorised→Captured transition. Deterministic additive rule engine. 95.4% test coverage. P99 < 200ms at 1,000+ TPS. |
| **recon-engine** | `.NET 8` `SQL Server` `Hangfire` | Transaction reconciliation pipeline — exact match, fuzzy match, configurable rules. Built for financial data integrity. |
| **kyc-service** | `.NET 8` | FICA-aligned digital onboarding. SA ID validation (Luhn + checksum), risk scoring, document verification pipeline. |

---

## Stack

**Core**

![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

---

## How I Build

- **Idempotency by Default** — Payment processing taught me that every operation must be safe to retry. At-least-once delivery is the norm, not an edge case.
- **State Machines over Ad-Hoc Logic** — Loan applications, payments, fraud verdicts — if it has states, it has a machine. Explicit transitions prevent impossible states.
- **Clean Architecture** — Domain and Application layers never reference infrastructure. Makes testing, swapping databases, or changing message brokers a config change, not a rewrite.
- **Test Coverage is Non-Negotiable** — RT-FDE at 95.4% coverage. Unit tests for domain logic, integration tests via Testcontainers for infrastructure. If it's not tested, it doesn't exist.
- **POPIA Compliance Designed In** — PII isolation, audit trails, data retention schedules. Not bolted on after the fact — designed into the domain model.
- **Containers from Day One** — Every project has a Dockerfile from the first commit. No "works on my machine."
- **Observability is a Feature** — Structured logging (Serilog), health checks, metrics. If it can't be monitored, it doesn't go to production.

---

## What I'm Building Toward

Remote backend engineering — fintech, SaaS, or any system where transactional integrity and distributed systems matter. Based in Johannesburg, South Africa.

---

<div align="center">

![Karabo's GitHub Stats](https://github-readme-stats.vercel.app/api?username=DynamicKarabo&show_icons=true&theme=tokyonight&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=DynamicKarabo&layout=compact&theme=tokyonight&hide_border=true)

</div>

---

## 📬 Reach Out

- 💼 [LinkedIn](https://linkedin.com/in/karabo-oliphant)
- 📧 [karabo.oliphant34@gmail.com](mailto:karabo.oliphant34@gmail.com)

> *"Ship fast. Sleep well. Test everything."*
