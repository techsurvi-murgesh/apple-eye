# 100 Interview Questions — AI-Native SDE-II Engineer, Shopify — 2026-10-13

Target profile: senior backend engineer (Go + Node.js/TypeScript), high-scale event-driven systems on Kafka/Redpanda, ClickHouse/MongoDB/PostgreSQL/Redis, AWS, background jobs and messaging services, AI-native engineering practice, plus shipped AI/LLM product experience.

## Go & Concurrency (1–14)

1. Explain goroutines and how they differ from OS threads.
2. What is the difference between buffered and unbuffered channels?
3. Explain `select` and how you avoid goroutine leaks.
4. What is the race condition? How do you detect and fix it?
5. Explain `sync.Mutex` vs `sync.RWMutex` vs `sync.WaitGroup`.
6. What is context cancellation and why does it matter in Go services?
7. How do you set goroutine and connection limits in Go?
8. Explain the difference between `errgroup` and manual `WaitGroup` usage.
9. What happens when a goroutine panics? How do you recover gracefully?
10. Explain memory allocation and GC pressure in Go. How do you reduce allocations?
11. How do you profile a Go service (pprof, trace, benchmarks)?
12. What is the difference between a worker pool and spawning per request?
13. How do you implement graceful shutdown with in-flight requests?
14. Explain `sync.Map` vs a map with a mutex. When is each correct?

## Node.js / TypeScript (15–28)

15. Explain the Node.js event loop and where blocking I/O hurts.
16. What is the difference between `setImmediate`, `process.nextTick`, and `setTimeout`?
17. Explain the microtask vs macrotask queues.
18. How do you handle CPU-heavy work in Node without blocking the loop?
19. What are streams in Node and when would you use them?
20. How do you implement graceful shutdown in a Node service?
21. Explain `async/await` and common concurrency pitfalls (sequential awaits, Promise.all).
22. What is an unhandled promise rejection and how do you prevent it?
23. How do you structure a large TypeScript codebase safely (types, strictness, boundaries)?
24. Explain BullMQ: queues, workers, concurrency, rate limiting, retries, flows.
25. How do you do rate limiting and backpressure in a Node API?
26. How would you debug a memory leak in Node?
27. What is the difference between Express, Fastify, and NestJS? When would you pick each?
28. How do you handle database connections and pool exhaustion in Node?

## Kafka / Redpanda (29–44)

29. What problem does Kafka solve? Explain topics, partitions, and offsets.
30. Explain delivery semantics: at-most-once, at-least-once, exactly-once.
31. What are consumer groups and why do you need them?
32. How do you guarantee ordering, and when can't you?
33. How do you choose the number of partitions?
34. Explain replication factor, leader election, and ISR.
35. What is a consumer group rebalance and how do you minimise churn?
36. Explain consumer lag: what causes it and how do you alert on it?
37. How do you implement idempotent processing on the consumer side?
38. What is a Dead Letter Queue and how do you replay from it?
39. Explain backpressure in a Kafka consumer and how to handle it.
40. How do you design a replay/reprocessing strategy for a downstream fix?
41. What is Kafka Connect and Schema Registry? When do you use them?
42. Kafka vs Redpanda vs SQS — when would you pick each?
43. How do you handle a poison pill message without blocking the partition?
44. How do you test a Kafka pipeline deterministically?

## Data Stores (45–60)

45. Design a data model for events in ClickHouse. Which engine and why?
46. Explain ORDER BY vs PARTITION BY in ClickHouse.
47. What are materialized views in ClickHouse and what are the trade-offs?
48. How do you deduplicate in ClickHouse (ReplacingMergeTree, FINAL, deduplication tokens)?
49. How do you diagnose a slow ClickHouse query? Talk about parts, marks, and prewhere.
50. How do you model documents in MongoDB, and how do you choose indexes?
51. Explain covering indexes and compound index ordering in MongoDB.
52. When do you embed vs reference a document in MongoDB?
53. Explain MVCC in PostgreSQL and how isolation levels affect correctness.
54. How do you tune a slow PostgreSQL query (EXPLAIN ANALYZE, indexes, statistics)?
55. How do you use Redis for caching, and how do you handle cache invalidation?
56. Explain rate limiting with Redis (token bucket, sliding window) and its concurrency safety.
57. How do you use Redis as a queue, and what are the trade-offs vs Kafka?
58. When would you choose Elasticsearch, ScyllaDB, or Cassandra over these?
59. Explain multi-tenant data modelling — shared schema, schema-per-tenant, or DB-per-tenant.
60. How do you do zero-downtime schema migration on a live table?

## APIs, Webhooks & Fault Tolerance (61–72)

61. How do you design an idempotent API for a messaging platform?
62. How do you handle duplicate and out-of-order webhook delivery from third parties?
63. How do you design a webhook dispatcher with retries and a dead-letter path?
64. Explain rate limiting from the caller's perspective (429, Retry-After, backoff with jitter).
65. How do you design a campaign scheduler that survives restarts?
66. Explain circuit breakers, bulkheads, and timeouts in a distributed system.
67. How do you do service-to-service authentication and authorization?
68. How do you version an API and deprecate it safely?
69. How do you implement pagination for very large result sets?
70. How do you propagate trace context across async boundaries?
71. What is partial failure in a workflow, and how do you make it recoverable?
72. How do you design for third-party rate limits you don't control?

## AWS & Operations (73–82)

73. Which AWS services would you use to run this stack, and why?
74. How do you deploy a Node/Go service on AWS safely (rolling vs blue/green)?
75. How do you manage infrastructure cost for a high-throughput event system?
76. How do you containerise a Go and a Node service in CI?
77. How does SQS + Lambda compare to a long-running consumer for bursty traffic?
78. How do you configure autoscaling based on queue depth, not just CPU?
79. Explain how you'd do zero-downtime schema and code deploys together.
80. What belongs in a production debugging runbook?
81. How do you use OpenTelemetry to trace a request across async consumers?
82. How do you detect and fix a memory leak in a long-running consumer?

## AI-Native Engineering & LLM Products (83–100)

83. What does AI-native mean to you, beyond using a coding assistant?
84. How do you use AI tools effectively for coding, testing, refactoring, and investigation?
85. How do you independently verify AI-generated code before it ships?
86. Describe an AI/LLM product or prototype you built. What did you personally build?
87. How does your system work beyond a single model API call?
88. How do you evaluate LLM output quality? What metrics and test sets do you use?
89. How do you handle hallucination in a customer-facing feature?
90. Explain structured outputs / function calling and when you prefer them over free text.
91. Explain RAG: chunking, embeddings, retrieval, reranking, and grounding.
92. How do you decide between RAG, fine-tuning, and prompting?
93. What are agent workflows, and how do you build tool-calling agents safely?
94. How do you prevent prompt injection in an agent that has tool access?
95. How do you protect sensitive data when calling an LLM API?
96. How do you control latency and cost of an LLM-powered feature?
97. How do you build an offline eval harness that gates prompt changes?
98. Explain MCP. What problem does it solve for AI tooling?
99. How do you debug a production issue where an LLM feature returns bad output?
100. Describe a hard production incident you owned. What did you change so it could not happen again?

---