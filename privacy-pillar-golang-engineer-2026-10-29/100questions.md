# 100 Interview Questions — Golang Engineer, Privacy Pillar

Target profile: Golang Developer building REST and gRPC services, scalable microservices, message-driven workflows, Gin applications, Temporal workflows, and PostgreSQL-backed systems with strong data structures, design patterns, concurrency, and production reliability.

## Go Language and Concurrency (1–15)

1. How does Go manage memory, and when would you avoid unnecessary allocations?
2. Explain goroutines, channels, and how they differ from threads.
3. What is the difference between buffered and unbuffered channels?
4. How do you prevent goroutine leaks in long-running services?
5. When would you use `sync.Mutex`, `sync.RWMutex`, and channels?
6. How does `context.Context` work, and why is it important for request lifecycles?
7. How would you implement worker pools in Go for a high-throughput service?
8. What happens when a channel is closed while receivers or senders are still active?
9. How do you use `select` to handle multiple channels and timeouts?
10. How would you implement rate limiting in Go?
11. How does Go's `defer` work, and what performance considerations does it have?
12. How do you avoid data races when sharing state across goroutines?
13. How would you use `errgroup` to manage concurrent operations?
14. What is the difference between a pointer and a value receiver?
15. How do you profile CPU, memory, and goroutine usage in a Go service?

## Gin, REST APIs, and gRPC (16–30)

16. Why use Gin for HTTP APIs, and what are its main performance characteristics?
17. How would you structure handlers, services, and repositories in a Gin application?
18. How do you implement request validation and custom error responses in Gin?
19. How do you design versioned REST APIs without breaking existing clients?
20. How would you secure REST endpoints with JWT or OAuth?
21. What makes a good API contract, and how do you document it?
22. How do REST APIs differ from gRPC in performance and developer experience?
23. How do you define protobuf messages and services for gRPC?
24. How would you implement unary, server-streaming, and client-streaming gRPC methods?
25. How do you handle gRPC deadlines, retries, and metadata?
26. How do you expose both REST and gRPC interfaces for the same service?
27. How would you implement middleware for authentication, logging, and tracing?
28. How do you handle pagination, filtering, and sorting in REST APIs?
29. How do you design idempotent APIs for create and update operations?
30. How would you version protobufs without breaking generated clients?

## Microservices and System Design (31–45)

31. What makes a microservice boundary well-defined?
32. How would you split a monolithic Go application into microservices?
33. How do services discover and communicate with one another?
34. How do you handle failures between microservices without cascading outages?
35. What patterns would you use for retries, circuit breakers, and timeouts?
36. How do you implement service-to-service authentication?
37. How would you design a consent-management service for a privacy platform?
38. How do you ensure data consistency across multiple services?
39. When would you use synchronous calls versus asynchronous messaging?
40. How do you design a service for high availability and horizontal scalability?
41. How do you handle graceful shutdown in a Go microservice?
42. How would you implement health checks and readiness probes?
43. How do you design API gateways and reverse proxies for microservices?
44. How do you handle schema evolution across service boundaries?
45. How would you design an audit trail for privacy and consent operations?

## RabbitMQ and Workflow Messaging (46–58)

46. Explain exchanges, queues, bindings, and routing keys in RabbitMQ.
47. How do you design reliable message publishing and consumption?
48. What is the difference between at-most-once, at-least-once, and exactly-once delivery?
49. How do you implement idempotent consumers?
50. How would you handle dead-letter queues and poison messages?
51. How do you ensure ordering or prevent race conditions in message consumers?
52. How do you handle retries with exponential backoff in RabbitMQ?
53. How do you scale consumers horizontally without duplicate processing?
54. What are the trade-offs between RabbitMQ and Kafka?
55. How would you design a workflow messaging system for long-running business processes?
56. How do you correlate messages across services for observability and tracing?
57. How do you prevent message loss during consumer restarts or deployments?
58. How do you monitor queue depth, consumer lag, and failed messages?

## Temporal Workflows (59–68)

59. What problem does Temporal solve compared with ordinary background jobs?
60. How do workflows, activities, and workers work in Temporal?
61. How do you write deterministic workflow code in Go?
62. How would you implement retries, timeouts, and compensation in Temporal?
63. How do you handle long-running workflows with signals and queries?
64. How do you version Temporal workflows safely?
65. How do you test workflows and activities independently?
66. How do you scale Temporal workers and handle activity failures?
67. When would you use Temporal instead of RabbitMQ alone?
68. How do you ensure workflow state is recoverable after a worker crash?

## PostgreSQL and ORM Frameworks (69–78)

69. How do you design normalized PostgreSQL schemas for consent-management data?
70. How do indexes affect query performance, and when can they hurt writes?
71. How do you analyze and optimize a slow PostgreSQL query?
72. What are transactions, isolation levels, and common concurrency anomalies?
73. How do you avoid N+1 query problems with an ORM?
74. How do you implement pagination efficiently in PostgreSQL?
75. How do you use database migrations safely in production?
76. How do you handle connection pooling and database connection limits?
77. How do you implement soft deletes and audit columns?
78. How would you design a backup and restore strategy for PostgreSQL?

## Data Structures, Design Patterns, and OOP (79–88)

79. How do slices, arrays, and maps differ in Go, and what are their performance implications?
80. How would you implement a custom data structure for a specific workload?
81. Which design patterns are most useful in Go services?
82. How do interfaces enable dependency injection in Go?
83. How do you avoid overusing inheritance-style thinking in Go?
84. How would you apply the repository pattern in a Go application?
85. How do you implement the factory and strategy patterns in Go?
86. How do you structure domain models around business rules?
87. How do you validate data at domain boundaries?
88. How do you refactor a service while preserving behavior and tests?

## Testing, Observability, and Production (89–95)

89. How do you write table-driven tests in Go?
90. How do you mock dependencies for unit tests?
91. What should integration tests cover for a microservice?
92. How do you instrument a Go service with metrics, logs, and traces?
93. How would you debug a production memory leak in a Go service?
94. How do you define and monitor SLOs for a backend service?
95. How do you handle configuration and secrets across environments?

## Behavioral and Scenario Questions (96–100)

96. Describe a complex Go microservice you designed end to end.
97. Tell me about a time you improved the performance or reliability of a service.
98. How would you handle a production incident involving RabbitMQ and downstream services?
99. How do you balance feature delivery with code quality and maintainability?
100. Why are you a strong fit for the Golang Engineer role at Privacy Pillar?
