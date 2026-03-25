# 🧪 Lab 01: Mastering HTTP with `curl`

In this lab, you will use `curl` to interact with a mock API and understand precisely how headers and methods affect the server response.

## 🛠 Prerequisites
Ensure you have `curl` installed. Run `curl --version` to check.

## 📝 Exercises

### 1. The Verbose GET
Fetch a resource and inspect the full header exchange.
```bash
curl -v https://jsonplaceholder.typicode.com/posts/1
```
> **Observation**: Look for `> GET` (Request) and `< HTTP/1.1 200 OK` (Response).

### 2. Custom Headers & Content Negotiation
Tell the server you prefer XML over JSON (if supported).
```bash
curl -H "Accept: application/xml" https://jsonplaceholder.typicode.com/posts/1
```

### 3. The Idempotent PUT
Update a resource. Note that running this multiple times results in the same state.
```bash
curl -X PUT -H "Content-Type: application/json" \
     -d '{"title": "Updated Title", "body": "bar", "userId": 1}' \
     https://jsonplaceholder.typicode.com/posts/1
```

### 4. Inspecting the `ETag` (Cache Control)
Run a HEAD request to see if the resource has changed without fetching the body.
```bash
curl -I https://jsonplaceholder.typicode.com/posts/1
```

---
[Return to Module Foundations](../README.md)
