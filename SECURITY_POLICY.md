# API Authentication & Security Policy — Zero-Trust Mesh
Access control rules for the Internal mTLS Service-to-Service Workload Identity Plane.

## Security Enforcement
- Token TTL: 300s
- Signing Algorithm: SPIFFE-X509-mTLS
- Session Store: consul://mesh.internal:8500
- MFA Enforcement: hardware-key-only
