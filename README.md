# yo 👋

**karabo** · backend engineer · johannesburg, SA 🇿🇦

i make .NET backends that handle real money.
idempotent by default. tested to death. containers always.

---

## the work

**lendflow** → lending platform with tenant isolation, state machines, and POPIA compliance designed in, not bolted on.

**payflow** → payment processing. HMAC-signed webhooks, merchant reconciliation, idempotent retries. money stuff.

**equilink** → institutional trading middleware. CQRS + event sourcing. 7-year regulatory WORM archiving. no cutting corners.

**recon-engine** → transaction matching pipeline. exact match → fuzzy match → rules. financial data integrity or bust.

**kyc-service** → FICA-aligned digital onboarding. SA ID validation (Luhn + checksum). document verification.

**k3s-cluster** → production Kubernetes on a single node. ArgoCD GitOps, cert-manager TLS, monitoring stack. deployed from commit to cluster.

---

## the stack

**core** — .NET · C# · SQL Server · PostgreSQL · Redis

**infra** — Docker · Kubernetes (k3s) · ArgoCD · Helm · GitHub Actions · cert-manager

---

## how i build

• **idempotent or nothing** — every operation survives retry. learned that the hard way.

• **state machines over spaghetti** — if it has states, it has a machine. no impossible states here.

• **test it or it doesn't ship** — 95.4% coverage on RT-FDE. unit tests for domain logic, integration via Testcontainers. if it's not tested, it doesn't exist.

• **containers from commit one** — "works on my machine" is not a sentence i say.

• **privacy by design** — POPIA isn't an afterthought. PII isolation, audit trails, retention schedules are in the domain model.

• **observability is a feature** — structured logging, health checks, metrics. if it can't be monitored, it stays local.

---

## currently

building: .NET backends + k3s GitOps pipeline
location: johannesburg, SA
target: remote backend — fintech, SaaS, or anywhere transactional integrity matters
vibe: "commit to main. CI builds it. ArgoCD ships it."

---

## 📬 reach out

[linkedin](https://linkedin.com/in/karabo-oliphant) · karabo.oliphant34@gmail.com
