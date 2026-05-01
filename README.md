<div align="center">

# **Karabo Oliphant**
### Backend Engineer · Johannesburg, South Africa 🇿🇦

[![GitHub followers](https://img.shields.io/github/followers/DynamicKarabo?style=for-the-badge&logo=github&color=0e75b6)](https://github.com/DynamicKarabo)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/karabo-oliphant)
[![Email](https://img.shields.io/badge/Email-Reach%20Out-red?style=for-the-badge&logo=gmail)](mailto:karabo@example.com)

</div>

---

> **I ship production systems.** .NET backends, Python ML services, deployed on Kubernetes. From payment processing to reinforcement learning agents — I build distributed systems that handle real data without falling over.

---

## 🚀 Shipped Projects

### ⚙️ Backend

| Project | Stack | What It Does |
|---------|-------|--------------|
| **LendFlow** | `.NET 8` `React` `SQL Server` `Redis` | Micro-lending platform with real-time credit scoring and loan lifecycle management |
| **PayFlow** | `.NET 8` `React` `SQL Server` `Redis` | Payment processing system with idempotency, retries, and transaction reconciliation |
| **recon-engine** | `.NET 8` `XGBoost` `SQL Server` `Hangfire` | Transaction reconciliation with ML-powered matching — Exact → Fuzzy → ML → RuleBased. **0.99 ROC AUC** |
| **EquiLink** | `.NET 8` `React` `CQRS` `Event Sourcing` `PostgreSQL` | Trading platform on event-driven architecture with full audit trails |
| **RT-FDE** | `.NET 8` `Redis` `xUnit` | Real-time fraud detection engine — **95.4% test coverage** |
| **kyc-service** | `.NET 8` `Azure Blob Storage` | Customer onboarding with document verification |

### 🧠 ML Systems

| Project | Stack | What It Does |
|---------|-------|--------------|
| **rl-trading-agent** | `Python` `PyTorch` `SB3` `FastAPI` `K8s` `GHCR` | PPO reinforcement learning trading agent deployed on **k3s Kubernetes** with multi-stage Docker slim build (4GB → 521MB), Prometheus/Grafana monitoring, MLflow tracking |
| **Feature Store Lite** | `Python` `FastAPI` `Pydantic` | 78 features across 3 views — centralized feature serving for ML inference, deployed as K8s microservice |
| **ml-platform** | `Python` `FastAPI` `PostgreSQL` `Docker` | Self-service MLOps platform — register, version, deploy, and monitor models via CLI or API |
| **ml-fraud-detection** | `Python` `Kafka` `MLflow` `MinIO` `DVC` `Prometheus` `Grafana` | Full MLOps pipeline with streaming data, experiment tracking, data versioning, drift detection — **72 passing tests** |
| **ML Monitoring** | `Prometheus` `Grafana` `Alertmanager` | Real-time observability for deployed models — metrics, drift, resource alerts |

### 🌐 Other

| Project | Stack | What It Does |
|---------|-------|--------------|
| **FD-Marketplace** | `Node.js` `React` `Kafka` `Stripe` `PostgreSQL` | Food delivery marketplace with microservices and payment orchestration |
| **EduTrack** | `Vite` `React` `TypeScript` `Tailwind` | Real-time class attendance and student tracking |

---

## 🛠️ Stack

**Backend**

![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)

**ML / Data**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-optimized-00FF00?style=for-the-badge&logo=python&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![k3s](https://img.shields.io/badge/k3s-FFC61C?style=for-the-badge&logo=k3s&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white)
![GHCR](https://img.shields.io/badge/GHCR-Registry-2D76B5?style=for-the-badge&logo=github&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

---

## ⚙️ How I Build

- **Test-Driven by Default** — Unit, integration, and contract tests before features hit staging. RT-FDE at **95.4% coverage** not by accident, by design.
- **CI/CD Native** — Every project ships with automated pipelines. No manual deploys. No "works on my machine."
- **Clean Architecture** — CQRS, Event Sourcing, and vertical slice architecture where the domain demands it. I optimize for readability at 2 AM during an incident.
- **Idempotency First** — Payment processing taught me that operations must be safe to retry. Every API I build expects at-least-once delivery and handles it gracefully.
- **Observability In** — Prometheus metrics, structured logging, Grafana dashboards, and health checks out of the box. If it can't be monitored, it's not production-ready.
- **Container-Native ML** — Multi-stage Docker builds slim ML images from 4GB to 521MB. Models versioned, deployed on **k3s Kubernetes**, pulled from **GHCR**.
- **From Notebook to Deployment** — Jupyter experiments → MLflow tracking → DVC data versioning → Docker image → Kubernetes rollout. No gaps.
- **Stack Choice is Strategic** — .NET for transactional integrity. Python for ML. Kafka for streaming. K8s for deployment. I pick the right tool for the constraints.

---

## 📈 GitHub Stats

<div align="center">

![Karabo's GitHub Stats](https://github-readme-stats.vercel.app/api?username=DynamicKarabo&show_icons=true&theme=tokyonight&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=DynamicKarabo&layout=compact&theme=tokyonight&hide_border=true)

</div>

---

## 📬 Let's Build Something

I'm open to **remote opportunities** and **contract work**.

- 💼 [LinkedIn](https://linkedin.com/in/karabo-oliphant)
- 🐦 [X / Twitter](https://twitter.com/DynamicKarabo)
- 📧 [karabo@example.com](mailto:karabo@example.com)

> *"Ship fast. Sleep well. Test everything."*
