# 03. Design Mastery: Building Elegant Contracts

Designing an API is easy. Designing an *elegant* API that lasts a decade is an art.

## 📖 Topics Covered

### 1. Resource-Oriented Design
*   **Naming Protocols**: Plural nouns, kebab-case vs snake_case.
*   **Sub-resources**: Relationships in the URI (e.g., `/users/{id}/orders`).

### 2. Evolution & Versioning
*   **URI Versioning**: `/v1/resource` (Classic).
*   **Header Versioning**: `X-API-Version` (Cleaner).
*   **Media Type Versioning**: `Accept: application/vnd.myapi.v1+json` (True REST).

### 3. Resilience & Control
*   **Idempotency**: Ensuring retries don't duplicate operations (e.g., `Idempotency-Key`).
*   **Pagination**: Cursor-based vs Offset-based.
*   **Rate Limiting**: Throttling strategies (Leaky Bucket vs Token Bucket).

---
[Return to Main Roadmap](../README.md)
