# GKE GitOps Platform

Enterprise-grade GitOps platform on Google Kubernetes Engine (GKE) built using Terraform, Terragrunt, Argo CD, Helm, GitHub Actions, and Google Cloud Platform.

This project demonstrates modern Platform Engineering practices including Infrastructure as Code (IaC), GitOps, multi-environment deployments, Kubernetes platform automation, CI/CD, observability, and cloud-native security.

---

## Objectives

* Provision cloud infrastructure using Terraform and Terragrunt
* Deploy and manage Kubernetes workloads using GitOps
* Implement multi-environment deployments (Dev → Staging → Production)
* Automate infrastructure and application delivery pipelines
* Demonstrate production-grade platform engineering practices
* Showcase enterprise Kubernetes architecture on GCP

---

## Technology Stack

### Cloud

* Google Cloud Platform (GCP)
* Google Kubernetes Engine (GKE)
* Artifact Registry
* Cloud Storage
* IAM & Service Accounts

### Infrastructure as Code

* Terraform
* Terragrunt

### Kubernetes

* Kubernetes
* Helm
* Argo CD

### CI/CD

* GitHub Actions

### Observability

* Prometheus
* Grafana
* Google Cloud Monitoring

---

## Repository Structure

```text
.
├── .github/
│
├── bootstrap/
│
├── docs/
│
├── gitops/
│
├── helm/
│
└── infrastructure/
    └── gcp/
        ├── _common/
        ├── _modules/
        ├── dev/
        ├── staging/
        ├── prod/
        └── root.hcl
```

---

## Environment Strategy

```text
Development
     │
     ▼
 Staging
     │
     ▼
 Production
```

Infrastructure and application changes are promoted through environments using pull requests and GitOps workflows.

---

## Infrastructure Layout

```text
infrastructure/gcp/

├── _common/
│   ├── cloud-vpc.hcl
│   ├── gke-cluster.hcl
│   ├── artifact-registry.hcl
│   └── monitoring.hcl
│
├── _modules/
│   ├── cloud-vpc
│   ├── gke-cluster
│   ├── artifact-registry
│   └── monitoring
│
├── dev/
├── staging/
└── prod/
```

---

## Branching Strategy

### Main Branch

Production-ready code.

### Develop Branch

Active development and integration branch.

### Pull Requests

All changes are introduced through Pull Requests to simulate enterprise development workflows.

---

## Planned Features

### Phase 1 – Foundation

* Repository Structure
* Terraform Modules
* Terragrunt Configuration
* Remote State Configuration

### Phase 2 – Core Infrastructure

* VPC
* Private GKE Cluster
* Artifact Registry
* IAM and Service Accounts

### Phase 3 – CI/CD

* GitHub Actions
* Terraform Validation
* Automated Infrastructure Deployment

### Phase 4 – GitOps

* Argo CD Installation
* App of Apps Pattern
* Environment Promotion

### Phase 5 – Platform Services

* Ingress Controller
* External DNS
* Cert Manager
* Secret Management

### Phase 6 – Observability

* Prometheus
* Grafana
* Alerting
* Dashboards

### Phase 7 – Security

* Workload Identity
* RBAC
* Policy Enforcement
* Image Scanning

---

## Architecture Vision

```text
GitHub
   │
   ▼
GitHub Actions
   │
   ▼
Terraform / Terragrunt
   │
   ▼
Google Cloud Platform
   │
   ▼
Google Kubernetes Engine
   │
   ▼
Argo CD
   │
   ▼
Kubernetes Applications
```

---

## Status

🚧 Work in Progress

This repository is being built incrementally to demonstrate real-world Cloud Platform Engineering and GitOps practices on Google Cloud Platform.
