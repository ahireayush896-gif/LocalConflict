# API Authentication & Security Policy — OAuth Gateway
Access control rules for the External OAuth2 & OIDC Token Exchange Gateway.

## Security Enforcement
- Token TTL: 900s
- Signing Algorithm: RS256-JWKS
- Session Store: redis://auth.internal:6379
- MFA Enforcement: required-for-admin
