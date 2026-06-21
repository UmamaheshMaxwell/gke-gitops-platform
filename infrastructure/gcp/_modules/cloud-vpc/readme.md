# Cloud VPC Module

Terraform module for provisioning a Google Cloud VPC network.

## Purpose

Creates the foundational networking layer for GKE clusters, including subnets, secondary IP ranges for pods and services, and firewall rules.

## Resources

- VPC network
- Subnets with primary and secondary IP ranges
- Cloud Router and Cloud NAT (optional)
- Firewall rules

## Usage

Referenced by Terragrunt configurations in `infrastructure/gcp/_common/cloud-vpc.hcl` and deployed per environment.

## Status

Work in progress — module implementation will be added in Phase 2 (Core Infrastructure).
