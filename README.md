### Hi, I'm Lahav 👋

DevOps & platform engineer. I design the infrastructure, delivery pipelines, and observability that keep production systems running, and I write the services that run on them.

I run **[rs-recruiting.com](https://rs-recruiting.com)** in production on my own: AWS infrastructure as code, keyless CI/CD, and full-stack telemetry for a live recruitment CRM.

---

#### 🚀 Featured: [rs-recruiting](https://github.com/lahavrud/rs-recruiting): production on AWS

<a href="https://github.com/lahavrud/rs-recruiting"><img src="https://raw.githubusercontent.com/lahavrud/rs-recruiting/main/docs/screenshots/aws-architecture.png" width="650" alt="RS Recruitment AWS architecture" /></a>

- **Infrastructure as code:** ECS Fargate, RDS, CloudFront + Lambda@Edge, SQS, EventBridge, and SSM-held secrets, all managed with **OpenTofu** across separate AWS accounts.
- **Delivery:** GitHub Actions authenticating to AWS over OIDC (no stored keys), with change detection and pytest against real Postgres. It deploys continuously to ECS behind a manual prod approval gate.
- **Observability:** Grafana Cloud (Loki / Tempo / Mimir) for logs, traces, and metrics, Sentry for errors, and CloudWatch alarms routed to SNS. Inspector2 scans images in ECR.
- **Supply chain & quality gates:** Ruff, ESLint, strict TypeScript, import-linter architecture contracts, and a weekly pip-audit.
- **The app itself:** an async FastAPI backend split into an API and an SQS worker, plus pgvector résumé matching and a Hebrew-first React UI.

**Kubernetes migration:** I re-platformed the same app onto **EKS** using Terragrunt across an AWS Organizations multi-account setup, Helm charts, and ArgoCD app-of-apps GitOps ([app + charts](https://github.com/lahavrud/rs-recruiting-course-app) · [GitOps repo](https://github.com/lahavrud/rs-recruiting-gitops)).

#### 🧰 Other things I've built

| | |
|---|---|
| [**homelab**](https://github.com/lahavrud/homelab) | Proxmox homelab that runs unattended while I'm abroad: 14 LXC containers on ZFS, GPU transcoding and ML, verified off-site backups, staged updates with automatic rollback, and incident write-ups. Started as Docker Compose on a 2 GB laptop |
| [**grisel**](https://github.com/lahavrud/grisel) | A general-purpose grid-selector TUI in Go (Bubble Tea) |
| [**aws-saa-c03-practice-exam**](https://github.com/lahavrud/aws-saa-c03-practice-exam) | Practice-exam platform for the AWS Solutions Architect Associate |

#### 🛠️ Stack

**Backend** &nbsp;
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)

**Frontend** &nbsp;
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**Cloud & Infra** &nbsp;
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![OpenTofu](https://img.shields.io/badge/OpenTofu-FFDA18?style=flat-square&logo=opentofu&logoColor=black)
![Terragrunt](https://img.shields.io/badge/Terragrunt-5C4EE5?style=flat-square&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white)

**Delivery & Ops** &nbsp;
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)
![Arch Linux](https://img.shields.io/badge/Arch_Linux-1793D1?style=flat-square&logo=archlinux&logoColor=white)

---

📫 [lahavrud@gmail.com](mailto:lahavrud@gmail.com) · 💼 [LinkedIn](https://www.linkedin.com/in/lahav-rudik-380329212/)
