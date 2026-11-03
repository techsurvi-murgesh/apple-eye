# 100 Interview Questions — Integration Engineer (Go / Event-Driven / AWS EKS)

## Go Language & Concurrency (1-15)

1. What are the key differences between goroutines and OS threads, and when would you choose one over the other?
2. How do channels work in Go, and what is the difference between buffered and unbuffered channels?
3. How does the `context` package work, and why is context propagation critical in integration services?
4. What is the difference between `context.Background()` and `context.TODO()`?
5. How do you handle cancellation and timeouts using context in a long-running integration flow?
6. What are common Go error-handling patterns, and how do you avoid repetitive `if err != nil` checks?
7. How do you define and use interfaces in Go, and why is interface-driven design important for integration adapters?
8. What is the difference between a value receiver and a pointer receiver in Go methods?
9. How does Go's garbage collector work, and what are common causes of memory leaks in Go services?
10. How do you detect and diagnose data races in Go code?
11. What is a `sync.Mutex` vs `sync.RWMutex`, and when would you use each in an integration service?
12. How do `sync.WaitGroup` and `sync.Once` work, and give a real use case for each.
13. What is the difference between a goroutine leak and a memory leak? How do you detect a goroutine leak?
14. How does the Go scheduler (GMP model) work at a high level?
15. What is `select` in Go, and how does it help with concurrent message handling?

## Go Web/API Frameworks, gRPC & REST (16-25)

16. Which Go web frameworks have you used (e.g., Gin, Echo, Chi, Fiber), and what are their trade-offs?
17. How do you structure a Go HTTP service for maintainability (handlers, services, repositories)?
18. What is gRPC, and how does it differ from REST in terms of performance and contract definition?
19. How do you define a gRPC service using Protocol Buffers, and how do you generate Go code from `.proto` files?
20. When would you choose gRPC over REST for an integration service, and vice versa?
21. How do you handle authentication and authorization in a Go REST API (JWT, OAuth2)?
22. How do you version a Go API, and what strategies ensure backward compatibility?
23. How do you implement middleware in a Go HTTP server (e.g., logging, tracing, auth)?
24. How do you test a Go HTTP handler without starting a real server (httptest)?
25. What is idempotency in an API, and how do you implement idempotent consumers in Go?

## Go Profiling & Tuning (26-30)

26. What tools do you use to profile Go applications (pprof, trace), and what metrics do you look at?
27. How do you profile CPU usage in a Go service, and what does a high CPU profile indicate?
28. How do you profile memory usage in Go, and how do you distinguish between inuse_space and alloc_space?
29. What is escape analysis in Go, and why does it matter for performance?
30. How do you tune Go service latency and concurrency for an integration workload?

## Enterprise Integration Patterns (Hohpe/Woolf) (31-45)

31. What are Enterprise Integration Patterns (EIP), and why are they relevant to integration services?
32. Explain the difference between synchronous and asynchronous integration, and when to use each.
33. What is the difference between orchestration and choreography in integration?
34. What is guaranteed delivery, and how do you achieve it with message queues?
35. What is the difference between exactly-once and at-least-once delivery, and why is exactly-once hard?
36. What is an idempotent consumer, and how do you implement one?
37. Describe the Message Channel pattern and how SQS/SNS implement it.
38. Describe the Message Router pattern (content-based router, recipient list).
39. Describe the Message Translator pattern and how it maps between source and target payloads.
40. What is the Claim Check pattern, and when would you use it for large payloads?
41. Describe the Circuit Breaker pattern and how it protects integration services from cascading failures.
42. What is the Retry/Backoff pattern, and how do you implement exponential backoff with jitter?
43. Describe the Saga pattern (choreography vs. orchestration) and compensation transactions.
44. What is the Outbox pattern, and how does it ensure reliable event publishing alongside database transactions?
45. Describe the Dead Letter Channel pattern and how SQS dead-letter queues implement it.

## Canonical Data Models (46-50)

46. What is a canonical data model in integration, and why is it useful?
47. When is a canonical model the right choice versus point-to-point or per-domain contracts?
48. How do you design a canonical schema layer for mapping source and target payloads?
49. What are the trade-offs of a canonical model (complexity, latency, coupling)?
50. How do you handle schema mapping and transformation between canonical and domain models?

## iPaaS Platforms (51-55)

51. Name iPaaS platforms you know (MuleSoft, Boomi, Workato, Azure Logic Apps, Informatica, TIBCO, webMethods).
52. What is connector development in an iPaaS, and how does it differ from custom code?
53. How do mapping and transformation work in iPaaS platforms?
54. How do you orchestrate multi-step integrations in an iPaaS versus custom code?
55. When would you choose an iPaaS over building custom integration services in Go?

## Design Patterns, Clean Architecture & SOLID (56-62)

56. What are creational, structural, and behavioral design patterns? Give one example of each.
57. What is Clean Architecture, and how do you apply it to an integration service?
58. Explain SOLID principles with a concrete example in Go.
59. What are domain boundaries, and how do you justify your design choices around them?
60. How do you separate concerns in a Go service (handlers, use cases, repositories/adapters)?
61. What is dependency injection in Go, and how do you implement it without a framework?
62. How do you structure a Go project for a multi-service integration platform?

## API Contracts & Schema Evolution (63-67)

63. What is an API contract, and why is it important for integration teams?
64. How do you document API and event schemas (OpenAPI, Protobuf, JSON Schema)?
65. What is schema evolution, and how do you maintain backward compatibility?
66. How do you handle breaking changes in an API contract without disrupting consumers?
67. What is versioning discipline, and how do you drive it across teams?

## Cloud & Platform — AWS EKS/Kubernetes (68-74)

68. What is EKS, and how does it differ from self-managed Kubernetes?
69. Describe Kubernetes Deployments, Services, and Ingress, and when to use each.
70. What are ConfigMaps and Secrets, and how do you manage configuration in Kubernetes?
71. What is HPA (Horizontal Pod Autoscaler), and how do you configure it?
72. How do you troubleshoot a live workload in Kubernetes (kubectl, logs, events, describe)?
73. What are health/readiness probes, and how do they affect rollout strategy?
74. Describe a Kubernetes rollout strategy (rolling update, blue/green, canary).

## Docker & Containerization (75-79)

75. What are multi-stage builds in Docker, and why do they matter for small runtime images?
76. How do you harden a Docker image (non-root user, minimal base, scanning)?
77. How do you optimize Docker image size for Go services (distroless, alpine, static binary)?
78. What is a container registry, and how do you manage image versions?
79. How do you secure container images in a CI/CD pipeline?

## SQS, SNS, Lambda — Event-Driven (80-86)

80. How does SQS work, and what is the difference between standard and FIFO queues?
81. How do you handle ordering and deduplication in SQS FIFO queues?
82. What is a dead-letter queue (DLQ), and how do you configure it in SQS?
83. What is a replay strategy for failed messages, and how do you implement it?
84. How does SNS work, and how does it differ from SQS?
85. How do you integrate SNS with Lambda for fan-out event delivery?
86. How does AWS Lambda work, and what are cold starts and provisioned concurrency?

## RDS — PostgreSQL/MySQL (87-91)

87. What is the difference between RDS PostgreSQL and RDS MySQL, and when would you choose each?
88. How do you design a database schema for an integration service (tables, indexes, relationships)?
89. How do you optimize data access (indexing, query tuning, connection pooling)?
90. What are transaction boundaries, and how do you manage them in Go (database/sql, sqlx, GORM)?
91. How do you handle database migrations safely in production?

## IAM, VPC, Secrets Manager, CloudWatch (92-95)

92. What is IAM, and how do you apply least-privilege principles to integration services?
93. What are VPC networking basics (subnets, security groups, routing)?
94. How do you manage secrets (Secrets Manager, Parameter Store) in AWS?
95. How do you use CloudWatch for monitoring and alerting on integration SLAs?

## AI in the Development Lifecycle (96-98)

96. What AI coding assistants have you used (Claude Code, GitHub Copilot, Cursor), and what did they accelerate?
97. Where have AI coding tools failed, and how did you validate their output?
98. What guardrails do you apply to AI-generated code (security review, licensing, hallucination checks)?

## Engineering Practice (99-100)

99. Describe your Git-based workflow and trunk/branching discipline.
100. What is your approach to test automation (unit, contract, integration) as part of definition of done?
