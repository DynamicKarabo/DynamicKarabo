# yo 👋

**karabo** · backend engineer · johannesburg, SA 🇿🇦

i make .NET backends that handle real money.
idempotent by default. tested to death. containers always.

---

## the work

**subject-rights-service** → POPIA compliance. DSAR management with a 30-day legal clock. Consent lifecycle tracking. Immutable audit trail over RabbitMQ. CQRS from request to event. *Privacy by design, enforced in code.*

**financial-event-engine** → Saga orchestrator for distributed financial transactions. Central coordinator guides multi-step payment flow with compensating rollbacks on failure. MassTransit + RabbitMQ + transactional outbox. *When money moves, every step counts.*

**lendflow** → lending platform with tenant isolation, state machines, and POPIA compliance designed in, not bolted on.

**payflow** → payment processing. HMAC-signed webhooks, merchant reconciliation, idempotent retries. money stuff.

**equilink** → institutional trading middleware. CQRS + event sourcing. 7-year regulatory WORM archiving. no cutting corners.

**recon-engine** → transaction matching pipeline. exact match → fuzzy match → rules. financial data integrity or bust.

**kyc-service** → FICA-aligned digital onboarding. SA ID validation (Luhn + checksum). document verification.

**dotnet-observability** → Centralised observability library for .NET services. OpenTelemetry tracing + metrics, Serilog structured logging. Pluggable NuGet components. *If it can't be monitored, it stays local.*

**k3s-cluster** → production Kubernetes on a single node. ArgoCD GitOps, cert-manager TLS, monitoring stack. deployed from commit to cluster.

---

## the stack

**core** — .NET · C# · SQL Server · PostgreSQL · Redis

**infra** — Docker · Kubernetes (k3s) · ArgoCD · Helm · GitHub Actions · cert-manager

**messaging** — RabbitMQ · MassTransit

---

## how i build

• **idempotent or nothing** — every operation survives retry. learned that the hard way.

• **state machines over spaghetti** — if it has states, it has a machine. no impossible states here.

• **test it or it doesn't ship** — unit tests for domain logic, integration via Testcontainers. if it's not tested, it doesn't exist.

• **containers from commit one** — "works on my machine" is not a sentence i say.

• **privacy by design** — POPIA isn't an afterthought. PII isolation, audit trails, retention schedules are in the domain model.

• **observability is a feature** — structured logging, health checks, metrics. if it can't be monitored, it stays local.

---

## currently

building: compliance systems, saga orchestrators, observability tooling
reading: distributed systems patterns
location: johannesburg, SA
vibe: "commit to main. CI builds it. CI tests it. CI ships it."

---

## 📬 reach out

[linkedin](https://linkedin.com/in/karabo-oliphant) · karabo.oliphant34@gmail.com
