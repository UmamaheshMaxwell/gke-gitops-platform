# Artifact Registry Module

Terraform module for provisioning Google Artifact Registry repositories.

## Purpose

Creates and configures Artifact Registry repositories for storing container images and other artifacts used by the GKE platform.

## Resources

- Artifact Registry repository
- IAM bindings for CI/CD and GKE workload access

## Usage

Referenced by Terragrunt configurations in `infrastructure/gcp/_common/artifact-registry.hcl` and deployed per environment.

## Status

Work in progress — module implementation will be added in Phase 2 (Core Infrastructure).
