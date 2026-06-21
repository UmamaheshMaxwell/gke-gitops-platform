# GitHub Actions Workflows

YAML workflow definitions for CI/CD automation in this repository.

## Purpose

Workflows in this directory validate changes, run infrastructure plans, and trigger deployments across environments. They integrate with Terraform, Terragrunt, and GCP using GitHub Actions.

## Planned Workflows

| Workflow | Trigger | Description |
|----------|---------|-------------|
| `terraform-validate.yml` | Pull request | Format check, lint, and validate Terraform/Terragrunt |
| `terraform-plan.yml` | Pull request | Generate and post Terragrunt plans per environment |
| `terraform-apply-dev.yml` | Merge to `develop` | Apply infrastructure changes to dev |
| `terraform-apply-staging.yml` | Manual / tag | Promote infrastructure to staging |
| `terraform-apply-prod.yml` | Manual / release | Apply infrastructure changes to production |

## Conventions

- Use reusable workflows or composite actions where logic is shared
- Require GCP authentication via Workload Identity Federation (no long-lived keys)
- Scope environment secrets and variables to GitHub Environments (`dev`, `staging`, `prod`)
- Fail fast on validation errors before running plans or applies

## Status

Work in progress — workflows will be added in Phase 3 (CI/CD).
