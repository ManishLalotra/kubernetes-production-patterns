# Kubernetes Production Topology

> This repository is a production reference implementation. It does not require or execute against an external Kubernetes cluster in this portfolio environment.

## Hardened Pod Security
- `runAsNonRoot: true` with dedicated UID 10001
- `readOnlyRootFilesystem: true`
- `capabilities.drop: ["ALL"]`
- Probes: Distinct Liveness (`/health`) and Readiness (`/ready`) endpoints.
