# 🧪 Lab 02: Deconstructing the JWT (JSON Web Token)

Digital identity in APIs relies heavily on JWTs. In this lab, you will learn to peel back the layers of a token.

## 🛠 Prerequisites
*   Web Browser or `node.js`.
*   [jwt.io](https://jwt.io) (Reference Tool).

## 📝 Exercises

### 1. The Anatomy of a Token
A JWT consists of three parts separated by dots: `Header.Payload.Signature`.
*   **Header**: Specifies the algorithm (HS256, RS256).
*   **Payload**: The "Claims" (User ID, Expiry, Roles).
*   **Signature**: Prove the token wasn't tampered with.

### 2. Base64 vs Encryption
**CRITICAL**: JWTs are encoded, NOT encrypted (usually). Anyone can decode your payload if they have the token.
*   Copy your token from a mock provider.
*   Paste it into `atob()` in your browser console:
```javascript
let payload = "eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ";
console.log(JSON.parse(atob(payload)));
```

### 3. Signing with a Secret
Use a tool to generate an HS256 token and verify it with a secret key.
> **Observation**: Changing even 1 character in the payload invalidates the signature. This is the core of API security.

---
[Return to Module Security](../README.md)
