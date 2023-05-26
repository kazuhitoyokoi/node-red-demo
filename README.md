node-red-demo
=============

```mermaid
sequenceDiagram
  participant Client
  participant REST API
  participant Database

  Client->>REST API: GET /api/data
  REST API->>Database: Query data
  Database-->>REST API: Return data
  REST API-->>Client: Return data
```