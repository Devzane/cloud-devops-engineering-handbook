# Cloud & DevOps Engineering Handbook

[![AWS](https://img.shields.io/badge/AWS-Cloud%20Architecture-232F3E?logo=amazon-aws&logoColor=white)](https://aws.amazon.com/)
[![Terraform](https://img.shields.io/badge/Terraform-1.5%2B-7B42BC?logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Ansible](https://img.shields.io/badge/Ansible-Automation-EE0000?logo=ansible&logoColor=white)](https://www.ansible.com/)
[![Docker](https://img.shields.io/badge/Docker-Multi--Stage-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)
[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?logo=github-actions&logoColor=white)](https://github.com/features/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A collection of in-depth technical writings, architecture deep-dives, and production playbooks covering Cloud Infrastructure, DevOps, Containerization, and Site Reliability Engineering.

---

## 📖 Series Catalog

### 🚀 Series 01: [Hands-On Cloud DevOps Engineering: Zero to Production](./series/01-hands-on-cloud-devops/SERIES-ROADMAP.md)

A comprehensive 12-part production engineering masterclass detailing the end-to-end design, provisioning, containerization, and continuous delivery of an enterprise financial platform (**ZeetaFin ERP**).

```text
 ┌────────────────────────────────────────────────────────────────────────┐
 │                      The Complete DevOps Stack                         │
 ├────────────────────────────────────────────────────────────────────────┤
 │ Phase 1: Infrastructure as Code & Host Configuration                   │
 │   • Modular Terraform (VPC, Subnet, Route Tables, Internet Gateway)    │
 │   • Hardened Ubuntu 24.04 LTS with IMDSv2 (SSRF protection)           │
 │   • Modular Ansible Role automating Docker CE & Systemd configuration  │
 │   • Zero-Drift Idempotency Verification                                │
 ├────────────────────────────────────────────────────────────────────────┤
 │ Phase 2: Application Containerization & Registry Distribution          │
 │   • Multi-stage Docker build for NestJS API (369 MB, non-root user)    │
 │   • Standalone Docker build for Next.js 14 Frontend (224 MB)           │
 │   • Local 3-tier orchestration with PostgreSQL 16 & health probes      │
 │   • Amazon ECR distribution with vulnerability scanning on push        │
 ├────────────────────────────────────────────────────────────────────────┤
 │ Phase 3: Continuous Integration & Automated Continuous Deployment      │
 │   • Least-privilege IAM bot user & encrypted GitHub Secrets            │
 │   • Declarative GitHub Actions CI/CD with Buildx layer caching         │
 │   • Remote EC2 deployment engine with zero-collision container swap    │
 │   • Multi-tier health probing and rapid rollback playbooks             │
 └────────────────────────────────────────────────────────────────────────┘
```

#### Phase 1: Cloud Infrastructure as Code & Host Configuration
* **Part 01:** [Building an Isolated AWS VPC and Network Foundation with Terraform](./series/01-hands-on-cloud-devops/phase1/01-aws-vpc-infrastructure-terraform.md)
* **Part 02:** [Hardening Cloud Compute: EC2 Provisioning, IAM Roles, and IMDSv2 Enforcement with Terraform](./series/01-hands-on-cloud-devops/phase1/02-ec2-iam-imdsv2-hardening.md)
* **Part 03:** [Immutable Host Configuration: Automating Docker CE Engine Setup with Ansible](./series/01-hands-on-cloud-devops/phase1/03-ansible-automation-docker.md)
* **Part 04:** [Production Verification: Ansible Idempotency Testing, Failure Recovery, and Infrastructure Auditing](./series/01-hands-on-cloud-devops/phase1/04-idempotency-testing-troubleshooting.md)

#### Phase 2: Enterprise Application Containerization & Amazon ECR
* **Part 05:** [Multi-Tier Application Architecture: Designing a Production Containerization Strategy](./series/01-hands-on-cloud-devops/phase2/01-enterprise-app-architecture-docker-overview.md)
* **Part 06:** [Hardening Node.js Workloads: Multi-Stage Docker Builds for NestJS REST APIs](./series/01-hands-on-cloud-devops/phase2/02-nestjs-backend-multi-stage-docker-build.md)
* **Part 07:** [Next.js in Production: Optimizing Frontend Containers with Standalone Builds and Alpine Linux](./series/01-hands-on-cloud-devops/phase2/03-nextjs-frontend-standalone-containerization.md)
* **Part 08:** [Local Stack Orchestration with Docker Compose and Amazon ECR Container Registry Distribution](./series/01-hands-on-cloud-devops/phase2/04-docker-compose-orchestration-and-ecr-push.md)

#### Phase 3: Continuous Integration & Automated Cloud Deployment
* **Part 09:** [Zero-Trust CI/CD Security: Least-Privilege IAM, Amazon ECR, and Hardened GitHub Secrets](./series/01-hands-on-cloud-devops/phase3/01-aws-iam-ecr-github-secrets-security.md)
* **Part 10:** [Declarative CI/CD Pipelines: Architecting GitHub Actions for Container Builds and ECR](./series/01-hands-on-cloud-devops/phase3/02-github-actions-ci-cd-workflow-architecture.md)
* **Part 11:** [Production Deployment Automation: Remote EC2 Orchestration and Zero-Downtime Rollouts](./series/01-hands-on-cloud-devops/phase3/03-ec2-remote-deployment-engine-automation.md)
* **Part 12:** [End-to-End Pipeline Verification, Health Probes, and Failure Recovery](./series/01-hands-on-cloud-devops/phase3/04-end-to-end-verification-observability-troubleshooting.md)

---

## 🌐 Publishing & Syndication Guide

All articles in this handbook include pre-configured metadata headers formatted for:
- [Dev.to](https://dev.to)
- [Hashnode](https://hashnode.com)
- [Medium](https://medium.com)
- [Substack](https://substack.com)
- [LinkedIn Articles](https://www.linkedin.com)

See the [Publishing Checklist & Social Media Templates](./series/01-hands-on-cloud-devops/SERIES-ROADMAP.md#publishing-checklist--best-practices) for copy-pasteable social hooks and canonical URL best practices.

---

## 📄 License

This repository and all technical articles are licensed under the [MIT License](LICENSE).
