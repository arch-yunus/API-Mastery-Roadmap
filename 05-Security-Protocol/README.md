# 05. Security Protocol: Hardening the Gateway

Security is not a feature; it is a fundamental property of high-authority APIs.

## 📖 Topics Covered

### 1. Authentication & Authorization
*   **OAuth 2.1**: Scopes, Grant Types, and Authorization Codes.
*   **OIDC (OpenID Connect)**: The identity layer on top of OAuth.
*   **JWT (JSON Web Tokens)**: Claims, Signature validation, and JWS/JWE.

### 2. The OWASP API Security Top 10
*   **BOLA (Broken Object Level Authorization)**: The #1 API vulnerability.
*   **BFLA (Broken Function Level Authorization)**: Accessing admin functions.
*   **Mass Assignment**: Uncontrolled updates to sensitive fields.

### 3. Defensive Configuration
*   **CORS**: Secure cross-origin resource sharing.
*   **CSP (Content Security Policy)**: Preventing XSS in hydrated responses.
*   **IP Whitelisting & VPN**: Corporate-grade API isolation.

## 🚀 Lab Exercises
*   [Lab 02: Deconstructing the JWT](labs/01-jwt-breakdown.md)

---
[Return to Main Roadmap](../README.md)
