# 100 Interview Questions — Software Development Engineer, Backend (Golang) — Fox Corporation

## Go Language & Concurrency (1-15)

1. What are the key differences between goroutines and OS threads, and when would you choose one over the other?
2. How do channels work in Go, and what is the difference between buffered and unbuffered channels?
3. How does the `context` package work, and why is context propagation critical in backend services?
4. What is the difference between `context.Background()` and `context.TODO()`?
5. How do you handle cancellation and timeouts using context in a long-running request?
6. What are common Go error-handling patterns, and how do you avoid repetitive `if err != nil` checks?
7. How do you define and use interfaces in Go, and why is interface-driven design important for backend components?
8. What is the difference between a value receiver and a pointer receiver in Go methods?
9. How does Go's garbage collector work, and what are common causes of memory leaks in Go services?
10. How do you detect and diagnose data races in Go code?
11. What is a `sync.Mutex` vs `sync.RWMutex`, and when would you use each in a backend service?
12. How do `sync.WaitGroup` and `sync.Once` work, and give a real use case for each.
13. What is a goroutine leak, and how do you detect and fix one?
14. How does the Go scheduler (GMP model) work at a high level?
15. What is `select` in Go, and how does it help with concurrent message handling?

## Go Web/API, gRPC & REST (16-25)

16. Which Go web frameworks have you used (e.g., Gin, Echo, Chi, Fiber), and what are their trade-offs?
17. How do you structure a Go HTTP service for maintainability (handlers, services, repositories)?
18. What is gRPC, and how does it differ from REST in terms of performance and contract definition?
19. How do you define a gRPC service using Protocol Buffers, and how do you generate Go code from `.proto` files?
20. When would you choose gRPC over REST for a backend service, and vice versa?
21. How do you handle authentication and authorization in a Go REST API (JWT, OAuth2)?
22. How do you version a Go API, and what strategies ensure backward compatibility?
23. How do you implement middleware in a Go HTTP server (e.g., logging, tracing, auth)?
24. How do you test a Go HTTP handler without starting a real server (httptest)?
25. What is idempotency in an API, and how do you implement idempotent consumers in Go?

## Go Profiling & Performance (26-30)

26. What tools do you use to profile Go applications (pprof, trace), and what metrics do you look at?
27. How do you profile CPU usage in a Go service, and what does a high CPU profile indicate?
28. How do you profile memory usage in Go, and how do you distinguish between inuse_space and alloc_space?
29. What is escape analysis in Go, and why does it matter for performance?
30. How do you tune Go service latency and concurrency for a high-throughput workload?

## Data Structures & Algorithms (31-40)

31. What is the time and space complexity of common data structure operations (array, hash map, tree, graph)?
32. When would you use a hash map versus a slice versus a linked list in a backend service?
33. How do you implement a rate limiter in Go, and what algorithms are available (token bucket, leaky bucket)?
34. How do you detect a cycle in a linked list or graph?
35. How do you implement a cache with LRU eviction in Go?
36. How do you find the k-th largest element in a stream efficiently?
37. How do you merge k sorted lists, and what is the complexity?
38. How do you design an efficient search for high-throughput log data?
39. How do you approach a coding problem during an interview (clarify, examples, brute force, optimize, code, test)?
40. Why are data structures and algorithms important for backend and distributed systems design?

## Backend System Design & APIs (41-50)

41. How do you design a URL shortening service, and what are the key trade-offs?
42. How do you design a chat/messaging system for millions of users?
43. How do you design a video streaming backend (like Tubi) for low-latency playback?
44. What is the difference between vertical and horizontal scaling, and when do you use each?
45. How do you design a rate-limiting system for APIs at scale?
46. How do you handle database schema migrations in production without downtime?
47. How do you design an API for high read throughput (caching, read replicas)?
48. How do you design an API for high write throughput (sharding, queues, batching)?
49. What is the CAP theorem, and how does it apply to distributed backend systems?
50. How do you ensure consistency in a distributed system (strong vs. eventual consistency)?

## Distributed Systems & Reliability (51-60)

51. What are the fallacies of distributed computing, and how do they affect backend design?
52. How do you handle partial failures in a distributed system?
53. What is the Circuit Breaker pattern, and how does it protect backend services?
54. What is the Retry/Backoff pattern, and how do you implement exponential backoff with jitter?
55. What is the Bulkhead pattern, and how does it isolate failures?
56. How do you implement idempotency in a distributed backend system?
57. What is the Saga pattern (choreography vs. orchestration) and compensation transactions?
58. What is the Outbox pattern, and how does it ensure reliable event publishing?
59. How do you handle distributed transactions, and what are the alternatives (2PC, eventual consistency)?
60. How do you design for fault tolerance and high availability in backend services?

## Cloud & AWS (61-70)

61. What AWS services have you used for backend systems (Lambda, SQS, SNS, API Gateway, RDS, S3, EC2)?
62. How does AWS Lambda work, and what are cold starts and provisioned concurrency?
63. How does SQS work, and what is the difference between standard and FIFO queues?
64. How do you handle ordering and deduplication in SQS FIFO queues?
65. What is a dead-letter queue (DLQ), and how do you configure it in SQS?
66. How does SNS work, and how do you integrate it with Lambda for fan-out event delivery?
67. What is Amazon RDS, and how do you choose between PostgreSQL and MySQL?
68. How do you design for high availability on AWS (Multi-AZ, Auto Scaling, ELB)?
69. How do you secure AWS resources (IAM, Security Groups, KMS, Secrets Manager)?
70. How do you monitor AWS backend services (CloudWatch, CloudTrail, X-Ray)?

## Databases & Data Modeling (71-78)

71. What is the difference between relational and NoSQL databases, and when would you choose each?
72. How do you design a database schema for a backend service (tables, indexes, relationships)?
73. How do you optimize data access (indexing, query tuning, connection pooling)?
74. What are transaction boundaries, and how do you manage them in Go (database/sql, sqlx, GORM)?
75. How do you handle database migrations safely in production?
76. What is database sharding, and when would you use it?
77. How do you use caching (Redis, Memcached) to improve backend performance?
78. How do you handle cache invalidation and consistency?

## Testing, Observability & CI/CD (79-85)

79. What is the testing pyramid (unit, integration, contract, end-to-end), and how do you apply it to backend services?
80. How do you write unit tests in Go (testing package, table-driven tests, mocking)?
81. How do you perform integration testing for backend services (test containers, test databases)?
82. What is contract testing, and how do you ensure API compatibility between services?
83. How do you implement observability from day one (structured logging, metrics, distributed tracing)?
84. How do you set up alerting on backend SLAs (latency, error rate, availability)?
85. How do you design a CI/CD pipeline for backend services (build, test, scan, deploy, rollback)?

## AI & LLM Integration (86-90)

86. What is a Large Language Model (LLM), and how do you integrate LLM capabilities into backend software?
87. How do you call LLM-based APIs from a Go backend, and how do you handle latency and cost?
88. What is prompt engineering, and how do you design prompt-driven workflows?
89. How do you validate and sanitize LLM outputs in a production backend?
90. How do you use AI-assisted development tooling (Claude Code, GitHub Copilot, Cursor) to accelerate delivery while maintaining quality?

## Ownership, Code Reviews & Best Practices (91-100)

91. What does end-to-end ownership mean for a backend engineer (design to production operations)?
92. How do you participate in code and design reviews while maintaining high engineering standards?
93. How do you break down complex technical problems into practical, risk-based solutions?
94. How do you collaborate with cross-functional teams to deliver backend capabilities?
95. How do you continuously improve system reliability, developer productivity, and engineering best practices?
96. How do you work independently and make sound technical decisions with minimal guidance?
97. How do you balance performance, reliability, scalability, and cost in backend design?
98. How do you handle production incidents and perform root-cause analysis?
99. How do you mentor junior developers and share knowledge within the team?
100. Why do you want to work at Fox Corporation, and how does your experience match this Bengaluru Backend (Golang) role?
