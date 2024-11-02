# Kustomize Demo with Cert-manager

This repository demonstrates how to use Kustomize with Cert-manager for Kubernetes configuration management.

## Overview

This demo shows how to:
- Structure Kubernetes manifests using Kustomize
- Configure Cert-manager for issuing certificates
- Manage different environments (dev, staging, prod) using overlays

## Prerequisites

- Kubernetes cluster
- kubectl installed
- Cert-manager controller installed
- Kustomize (built into kubectl v1.14+)

## Directory Structure

.
├── base/                   # Base configurations
│   ├── base-install.yaml
│   ├── IAMCustomRole.yaml
│   ├── IAMPolicyMember.yaml
│   ├── IAMServiceAccount.yaml
│   └── kustomization.yaml
└── components/replacements              # Replacement configurations
│                  └── kustomization.yaml
└── overlays/              # Environment-specific configurations
    ├── dev/
    ├── stg/

