# Ervin Wallin

**Cloud & DevOps Engineer**  
[LinkedIn](https://linkedin.com/in/ervin-wallin) | [GitHub](https://github.com/szelese)

---

[![CKAD](https://img.shields.io/badge/Kubernetes-CKAD%20Certified-326CE5?style=flat-square&logo=kubernetes)](https://www.credly.com/badges/bfca75d3-7d7c-41df-8eda-753720505555/linked_in_profile)
[![AWS Certified Developer](https://img.shields.io/badge/AWS%20Certified%20Developer-Associate-FF9900?style=flat-square&logo=amazonaws)](https://www.credly.com/badges/993fe86f-e57e-4982-b356-b37b72961562)
[![Terraform Associate](https://img.shields.io/badge/HashiCorp%20Terraform-Associate-7B42BC?style=flat-square&logo=terraform)](https://www.credly.com/badges/da685d53-d623-402f-9994-b4fce26321f2)

[![v3 Kubernetes](https://img.shields.io/badge/v3-Kubernetes%20Native-326CE5?style=flat-square&logo=kubernetes)](https://github.com/szelese/v3-k8s-core)
[![v2 44ms Latency](https://img.shields.io/badge/Latency-44ms-blue?style=flat-square)](https://github.com/szelese/v2-agnostic-lambda-core)
[![v1 NIÜ Award](https://img.shields.io/badge/NIÜ-Awarded-FF9900?style=flat-square)](https://github.com/szelese/ci-cd-gha-aws)

---

## Cloud Architecture Evolution

**From PaaS → Serverless → Kubernetes-native delivery**  
2025–2026 | BSc Computer Science

| Version | Architecture | Technologies | Key Achievements |
|---------|--------------|--------------|------------------|
| **v1** | Django Monolith | Elastic Beanstalk, GitHub Actions | NIÜ/HSUP selected project, automated CI/CD |
| **v2** | Cloud-agnostic Serverless Core | Lambda, Docker, Hexagonal | 63% faster (120ms → 44ms), OWASP ZAP 0 alerts |
| **v2.1** | Full IaC Layer | Terraform, OIDC | Zero manual steps, least-privilege IAM |
| **v3** | **Kubernetes-native Runtime** | FastAPI, Docker, kind, Helm, Kustomize | Local K8s baseline, Ingress, HPA, NetworkPolicy, runtime hardening, CI |

The portfolio shows a deliberate progression: starting from traditional PaaS, advancing to high-performance cloud-agnostic serverless, adding full infrastructure automation, and now extending into container orchestration with Kubernetes.

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

This project is intentionally presented as a **local Kubernetes runtime portability baseline**, not as a full production platform yet.

---

### v2.1 – Full Terraform IaC Layer

[github.com/szelese/v2.1-agnostic-lambda-core-terraform](https://github.com/szelese/v2.1-agnostic-lambda-core-terraform)

A Terraform-based infrastructure automation layer around the v2 serverless core.

Key features:

- Fully automated AWS infrastructure provisioning
- Terraform-managed IAM, ECR, Lambda, CloudWatch alarms and SNS notifications
- GitHub Actions deployment workflow
- GitHub OIDC authentication
- Least-privilege IAM design
- Automatic GitHub Secrets management
- Smart smoke tests after deployment
- Zero manual infrastructure steps

---

### v2 – Agnostic Serverless Lambda Core

[github.com/szelese/v2-agnostic-lambda-core](https://github.com/szelese/v2-agnostic-lambda-core)

A cloud-agnostic Python application core adapted to AWS Lambda container runtime.

Key features:

- Hexagonal / clean architecture style separation
- Environment-agnostic business logic
- Dockerized Lambda runtime
- Performance improvement from approximately 120 ms to 44 ms average response time
- Around 63% faster response time compared to the original v1 system
- OWASP ZAP security audit with zero alerts
- Automated tests and validation pipeline

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
Least-privilege • Non-root containers • Prometheus metrics • Structured logging

**Architecture**  
Hexagonal design • Cloud-agnostic core

---

## Certifications

- Certified Kubernetes Application Developer — CKAD
- AWS Certified Developer – Associate
- HashiCorp Certified: Terraform Associate
- AWS Certified Cloud Practitioner

---

**Open to new opportunities** in Hungary & EU & worldwide
**Cloud • DevOps • Platform Engineering • Infrastructure as Code** roles

📩 **[ervin.wallin at gmail dot com](mailto:ervin.wallin@gmail.com)** | Let's build scalable, secure and fully reproducible cloud systems together!

---
*20 years in high-stakes logistics → reliability-first approach to cloud infrastructure.* 
---
![Profile views](https://komarev.com/ghpvc/?username=szelese&color=0e75b6&style=flat-square&label=Profile+views)  
© 2026 Ervin Wallin
