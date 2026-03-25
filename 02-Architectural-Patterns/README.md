# 02. Architectural Patterns: Diverse Communication Strategies

While REST is the industry standard, modern systems often require alternatives like GraphQL for flexibility or gRPC for performance.

## 📖 Topics Covered

### 1. GraphQL
*   **The Schema-First Approach**: Designing types, queries, and mutations.
*   **The Resolver Pattern**: How queries map to data sources.
*   **Performance**: Solving the N+1 problem with DataLoaders.

### 2. gRPC
*   **Protocol Buffers (Protobuf)**: Language-neutral binary serialization.
*   **Unidirectional vs Bidirectional Streaming**: Powering high-throughput service-to-service communication.
*   **Code Generation**: Using `protoc`.

### 3. Real-Time & Event-Driven
*   **Webhooks**: Reverse APIs for automated notifications.
*   **WebSockets**: Bi-directional full-duplex communication.
*   **SSE (Server-Sent Events)**: One-to-many event streaming for dashboards.

## 🚀 Lab Exercises
*   [Lab 03: GraphQL vs REST (Analysis)](labs/01-graphql-vs-rest.md)

---
[Return to Main Roadmap](../README.md)
