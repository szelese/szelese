# Ervin Wallin

**Cloud & DevOps Engineer**  
[LinkedIn](https://linkedin.com/in/ervin-wallin) | [GitHub](https://github.com/szelese)

---

[![CKAD](https://img.shields.io/badge/Kubernetes-CKAD%20Certified-326CE5?style=flat-square&logo=kubernetes)](https://www.credly.com/badges/bfca75d3-7d7c-41df-8eda-753720505555/linked_in_profile)
[![AWS Certified Developer](https://img.shields.io/badge/AWS%20Certified%20Developer-Associate-FF9900?style=flat-square&logo=amazonaws)](https://www.credly.com/badges/993fe86f-e57e-4982-b356-b37b72961562)
[![Terraform Associate](https://img.shields.io/badge/HashiCorp%20Terraform-Associate-7B42BC?style=flat-square&logo=terraform)](https://www.credly.com/badges/da685d53-d623-402f-9994-b4fce26321f2)

---

## Open-Source Contributions

### OpenTelemetry Helm Charts
**PR #2365** (merged) – Backward-compatible migration for renamed OTLP exporters (`otlp` → `otlp_grpc`, `otlphttp` → `otlp_http`)
- Rewrote exporter definitions and pipeline references while preserving named instances
- Added deprecation warnings, Helm unit and integration test coverage, and upgrade documentation
- Resolved merge conflicts and fixed a failing collector test on a local kind cluster

https://github.com/open-telemetry/opentelemetry-helm-charts/pull/2365

### Grafana Helm Chart Toolbox
**PR #146** (merged) – Added values.yaml validation before running documentation and schema generators
- Added regression tests for both `--file` and `--chart` modes
- Incorporated maintainer feedback by bumping both generators to 0.3.0 and updating their changelogs

https://github.com/grafana/helm-chart-toolbox/pull/146

---

## Cloud Architecture Evolution

**From PaaS → Serverless → Infrastructure as Code → Kubernetes-native delivery**
2025–2026 | BSc Computer Science

| Version | Architecture | Technologies | Key Achievements |
|---------|--------------|--------------|------------------|
| **v1** | Django Monolith | Elastic Beanstalk, GitHub Actions | Selected for further development by NIÜ/HSUP; automated CI/CD |
| **v2** | Cloud-agnostic Serverless Core | Lambda, Docker, Hexagonal | Documented median latency reduction (~120 ms → 44 ms); ZAP scan with 0 alerts in the recorded scenario |
| **v2.1** | Terraform IaC Layer | Terraform, GitHub OIDC | Repeatable AWS provisioning and automated application deployment |
| **v3** | **Kubernetes-native Runtime** | FastAPI, Docker, kind, Helm, Kustomize | kind-based Kubernetes baseline reproduced on AWS EC2, Ingress, HPA, NetworkPolicy, runtime hardening, CI |

The portfolio shows a deliberate progression: starting from traditional PaaS, advancing to cloud-agnostic serverless, adding Terraform-managed infrastructure, and extending into container orchestration with Kubernetes.

**Next milestone (v3.1):** Terraform-managed AWS EKS, ECR, GitHub OIDC and Helm-based deployment path.

---

## Highlighted Projects

### v3 – Kubernetes-Native Core

[github.com/szelese/v3-k8s-core](https://github.com/szelese/v3-k8s-core)

A Kubernetes-native delivery project that extends my earlier serverless portfolio into container orchestration.

Key features:

- Isolated Python business core with FastAPI HTTP adapter
- Non-root Docker runtime with Kubernetes security hardening (read-only filesystem, dropped capabilities)
- Local Kubernetes with `kind`, Kustomize and reusable Helm chart
- Ingress, Horizontal Pod Autoscaler, NetworkPolicy
- Prometheus-compatible `/metrics` endpoint + structured JSON logging
- Full GitHub Actions CI (pytest, Trivy scan, smoke tests, Helm validation)

This project is intentionally presented as a **local Kubernetes runtime portability baseline, reproduced locally and on a fresh AWS EC2 host using kind**, not as a production Kubernetes platform.

---

### v2.1 – Full Terraform IaC Layer

[github.com/szelese/v2.1-agnostic-lambda-core-terraform](https://github.com/szelese/v2.1-agnostic-lambda-core-terraform)

A Terraform-based infrastructure automation layer around the v2 serverless core.

Key features:

- Repeatable AWS infrastructure provisioning with Terraform
- Terraform-managed IAM, ECR, Lambda, CloudWatch alarms and SNS notifications
- GitHub Actions deployment workflow
- GitHub OIDC authentication
- Least-privilege IAM design
- Automatic GitHub Secrets management
- Smart smoke tests after deployment
- Initial infrastructure provisioning through `terraform apply`; subsequent application deployments are automated

---

### v2 – Agnostic Serverless Lambda Core

[github.com/szelese/v2-agnostic-lambda-core](https://github.com/szelese/v2-agnostic-lambda-core)

A cloud-agnostic Python application core adapted to AWS Lambda container runtime.

Key features:

- Hexagonal / clean architecture style separation
- Environment-agnostic business logic
- Dockerized Lambda runtime
- Documented median latency reduction from approximately 120 ms to 44 ms under the recorded Locust test scenario
- OWASP ZAP scan with zero alerts in the recorded test scenario
- GitHub Actions quality gate and version-aware post-deployment smoke test

---

### v1 – CI/CD with AWS Elastic Beanstalk

[github.com/szelese/ci-cd-gha-aws](https://github.com/szelese/ci-cd-gha-aws)

The original monolithic Django project and deployment baseline.

Key features:

- GitHub Actions CI/CD pipeline
- AWS Elastic Beanstalk deployment
- OIDC-based AWS authentication
- Automated deployment workflow
- Post-deploy hooks for database migration and static file collection
- Selected for further development by the Hungarian National Innovation Agency / HSUP

---

## Core Competencies

**Cloud & Infrastructure**  
AWS (Lambda, ECR, IAM, CloudWatch, Elastic Beanstalk) • Terraform IaC

**Kubernetes & Containers**  
Docker • FastAPI • kind • Kustomize • Helm • Ingress • HPA • NetworkPolicy • Security contexts

**CI/CD & Automation**  
GitHub Actions + OIDC • Trivy scanning • Smoke testing • Helm validation

**Security & Observability**  
Least-privilege • Non-root containers • Prometheus-compatible metrics • Structured logging

**Architecture**  
Hexagonal design • Cloud-agnostic core

---

## Certifications

- Certified Kubernetes Application Developer — CKAD
- AWS Certified Developer – Associate
- HashiCorp Certified: Terraform Associate
- AWS Certified Cloud Practitioner

---

**Open to Cloud, DevOps, Platform Engineering and Infrastructure as Code roles** in Hungary, the EU and remote international teams.

📩 **[ervin.wallin at gmail dot com](mailto:ervin.wallin@gmail.com)** | Let's build reliable, secure and reproducible cloud systems together!

---
*20 years in high-stakes logistics → reliability-first approach to cloud infrastructure.*

![Profile views](https://komarev.com/ghpvc/?username=szelese&color=0e75b6&style=flat-square&label=Profile+views)  
© 2026 Ervin Wallin
