# API Authentication & Security Policy — Zero-Trust Mesh & OAuth Gateway
Access control rules for the Internal mTLS Service-to-Service Workload Identity Plane and External OAuth2 & OIDC Token Exchange Gateway.

## Internal mTLS Service-to-Service Security Enforcement
- Token TTL: 300s
- Signing Algorithm: SPIFFE-X509-mTLS
- Session Store: consul://mesh.internal:8500
- MFA Enforcement: hardware-key-only

## External OAuth Gateway Security Enforcement
- Token TTL: 900s
- Signing Algorithm: RS256-JWKS
- Session Store: redis://auth.internal:6379
- MFA Enforcement: required-for-admin
