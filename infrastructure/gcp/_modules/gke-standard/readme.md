# GKE Standard Module

Terraform module for provisioning a Google Kubernetes Engine (GKE) standard cluster.

## Purpose

Creates a private GKE cluster with node pools, workload identity, and platform-level configuration required for GitOps workloads.

## Resources

- GKE cluster (standard mode)
- Node pools
- Workload Identity bindings
- Cluster add-ons and network policy configuration

## Usage

Referenced by Terragrunt configurations in `infrastructure/gcp/_common/gke-cluster.hcl` and deployed per environment.

## Status

Work in progress — module implementation will be added in Phase 2 (Core Infrastructure).
