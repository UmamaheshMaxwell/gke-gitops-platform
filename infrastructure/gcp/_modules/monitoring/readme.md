# Monitoring Module

Terraform module for provisioning Google Cloud Monitoring and observability resources.

## Purpose

Sets up monitoring infrastructure including notification channels, alert policies, and integrations with Prometheus and Grafana deployed on the cluster.

## Resources

- Cloud Monitoring notification channels
- Alert policies
- Uptime checks and dashboards (optional)
- IAM bindings for monitoring agents

## Usage

Referenced by Terragrunt configurations in `infrastructure/gcp/_common/monitoring.hcl` and deployed per environment.

## Status

Work in progress — module implementation will be added in Phase 6 (Observability).
