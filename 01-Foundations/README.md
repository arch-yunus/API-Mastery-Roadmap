# 01. Foundations: The Core Mechanics

This module covers the essential protocols and standards that power 99% of modern web communication. Understanding these is non-negotiable for anyone aspiring to be an API Master.

## 📖 Topics Covered

### 1. HTTP Protocol (The Heartbeat)
*   **Statelessness**: Why it matters for scalability.
*   **HTTP Methods**: Beyond GET/POST (PUT vs PATCH, HEAD, OPTIONS).
*   **Headers**: Content-Type, Accept, Cache-Control, ETag.

### 2. Status Codes (The Language of APIs)
| Range | Category | Purpose |
| :--- | :--- | :--- |
| **1xx** | Informational | Protocol switching, processing. |
| **2xx** | Success | Everything went right. (201 for POST is a must!) |
| **3xx** | Redirection | Resources moved. |
| **4xx** | Client Error | The requester broke the contract. |
| **5xx** | Server Error | The system failed internally. |

### 3. REST vs SOAP
*   **REST**: Architectural style, stateless, resource-based.
*   **SOAP**: Protocol-based, strict XML, built-in ACID compliance.

## 🚀 Lab Exercises
*   [Lab 01: Mastering HTTP with curl](labs/01-curl-commands.md)
