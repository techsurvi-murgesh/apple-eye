# 100 Interview Questions — Golang Full Stack Developer (Persistent Systems) — 2026-11-03

Target stack: Golang backend, React.js frontend, RESTful APIs, microservices, AWS/Azure, MySQL/PostgreSQL, MongoDB, Docker, Kubernetes, CI/CD, Git, Agile/Scrum.

## Golang Backend (1-20)

1. What are the key features of Go that make it suitable for backend services?
2. How do goroutines differ from OS threads, and how does the Go scheduler manage them?
3. How do channels work in Go, and when do you use buffered vs unbuffered channels?
4. How do you handle synchronization in Go (mutexes, WaitGroups, sync.Once, atomic)?
5. Explain Go interfaces and how they enable polymorphism without inheritance.
6. How does Go error handling differ from exceptions, and how do you propagate errors idiomatically?
7. How do you structure a Go project (package layout, cmd vs internal, go.mod)?
8. How do you write and run tests in Go, and what is table-driven testing?
9. How do you use pprof and benchmarks to profile CPU, memory, and goroutine usage?
10. How do you handle context cancellation, timeouts, and deadlines in Go services?
11. How do you build a REST API in Go (standard library net/http vs frameworks like Gin, Chi, Echo)?
12. How do you implement middleware in Go (logging, auth, recovery, CORS)?
13. How do you version and document Go APIs (OpenAPI/Swagger, godoc)?
14. How do you manage dependencies in Go (Go modules, go.sum, vendoring)?
15. How do you generate type-safe SQL in Go (sqlc, Goose migrations)?
16. How do you handle JSON serialization/deserialization in Go (encoding/json, struct tags)?
17. How do you implement graceful shutdown of an HTTP server in Go?
18. How do you secure a Go API (JWT, OAuth2, rate limiting, input validation)?
19. How do you connect Go to PostgreSQL and MongoDB (database/sql, mongo-driver)?
20. What are common Go concurrency pitfalls (race conditions, channel leaks, goroutine leaks)?

## React.js Frontend (21-40)

21. What is the React component lifecycle, and how do functional components use hooks instead?
22. How do useState and useEffect work, and what are common pitfalls with useEffect dependencies?
23. How do you handle forms and controlled components in React?
24. How do you lift state up vs use Context API vs Redux for state management?
25. How do you optimize React performance (React.memo, useMemo, useCallback, code splitting)?
26. How do you fetch data in React (useEffect, React Query/SWR, loading and error states)?
27. How do you handle routing in React (React Router, nested routes, protected routes)?
28. How do you build reusable, accessible React components (prop types, ARIA, composition)?
29. How do you style React applications (CSS modules, styled-components, Tailwind CSS)?
30. How do you handle authentication in React (JWT storage, token refresh, private routes)?
31. How do you integrate a React frontend with a Go backend REST API (fetch/axios, CORS)?
32. How do you handle file uploads and image optimization in React?
33. How do you test React components (Jest, React Testing Library, user-event)?
34. How do you handle forms validation in React (React Hook Form, Yup/Zod)?
35. How do you implement real-time features in React (WebSockets, SSE, polling)?
36. How do you optimize bundle size and load performance in a React app?
37. How do you handle errors globally in React (Error Boundaries)?
38. How do you manage environment variables and config in a React build?
39. How do you ensure responsive, mobile-first UI in React?
40. What are the differences between class components and functional components with hooks?

## RESTful APIs & Microservices (41-60)

41. What are the REST constraints, and how do you design resource-oriented URLs?
42. How do you use HTTP methods and status codes correctly in REST APIs?
43. How do you design API versioning strategy (URL versioning, header versioning)?
44. How do you handle pagination, filtering, and sorting in REST APIs?
45. How do you implement idempotency in API design?
46. How do you secure REST APIs (JWT, OAuth2, API keys, scopes)?
47. How do you document REST APIs (OpenAPI/Swagger, Postman collections)?
48. How do you handle CORS in a full-stack application?
49. What is the difference between REST and gRPC/GraphQL, and when do you use each?
50. What are microservices, and what are the benefits and challenges over monoliths?
51. How do you decompose a monolith into microservices (bounded contexts)?
52. How do services communicate in microservices (synchronous REST/gRPC vs asynchronous messaging)?
53. How do you handle distributed transactions in microservices (Saga pattern, two-phase commit)?
54. How do you implement service discovery and load balancing?
55. How do you manage shared data vs database-per-service in microservices?
56. How do you handle API gateway concerns (routing, auth, rate limiting, transformation)?
57. How do you implement health checks and readiness/liveness probes?
58. How do you version microservices and handle breaking changes?
59. How do you trace requests across microservices (correlation IDs, distributed tracing)?
60. How do you test microservices (contract testing, consumer-driven contracts)?

## Databases (61-80)

61. How do you design a relational database schema (normalization vs denormalization)?
62. How do you choose indexes in PostgreSQL/MySQL, and how do you analyze query plans (EXPLAIN)?
63. How do you optimize slow queries (indexing, query rewriting, avoiding N+1)?
64. How do you handle database transactions and isolation levels?
65. How do you design for high concurrency in relational databases (connection pooling, read replicas)?
66. How do you migrate database schema with zero downtime (online migrations, backward-compatible changes)?
67. When do you choose NoSQL (MongoDB) over relational (PostgreSQL/MySQL)?
68. How do you model data in MongoDB (embedding vs referencing, document design)?
69. How do you index MongoDB collections and analyze query performance?
70. How do you handle transactions and ACID guarantees in MongoDB?
71. How do you back up and restore PostgreSQL and MongoDB?
72. How do you secure databases (encryption at rest/in transit, least-privilege users)?
73. How do you handle database connection management in Go applications?
74. How do you implement caching with Redis alongside a database?
75. How do you handle database seeding and test data management?
76. How do you monitor database performance (slow query log, CPU, memory, connections)?
77. How do you handle partial failures in multi-database writes?
78. How do you design for read-heavy vs write-heavy workloads?
79. How do you implement soft deletes and audit trails in a database?
80. How do you choose between SQL and NoSQL for a given product requirement?

## Cloud, DevOps & Agile (81-100)

81. How do you deploy a Go+React application on AWS or Azure (compute, storage, networking)?
82. How do you containerize an application with Docker (multi-stage builds, small images)?
83. How do you orchestrate containers with Kubernetes (Pods, Deployments, Services, Ingress)?
84. How do you manage Kubernetes resources (ConfigMaps, Secrets, HPA, PodDisruptionBudgets)?
85. How do you implement CI/CD pipelines (build, test, scan, deploy, rollback)?
86. How do you use Git in collaborative workflows (branching strategy, PRs, code reviews)?
87. How do you manage environment variables and secrets in CI/CD (GitHub Secrets, Azure Key Vault, AWS Secrets Manager)?
88. How do you monitor and log full-stack applications (metrics, logs, traces, dashboards)?
89. How do you set up alerting and on-call for production incidents?
90. How do you perform root cause analysis for application issues?
91. How do you ensure application security (OWASP top 10, input validation, dependency scanning)?
92. How do you handle blue/green or canary deployments?
93. How do you write and maintain technical documentation and runbooks?
94. How do you participate in Agile ceremonies (sprint planning, stand-ups, reviews, retrospectives)?
95. How do you estimate and break down full-stack stories in Scrum?
96. How do you handle changing requirements mid-sprint?
97. How do you perform code reviews and enforce coding standards?
98. How do you balance speed vs technical debt in delivery?
99. How do you collaborate with QA, DevOps, and product owners in distributed teams?
100. What engineering excellence initiatives would you introduce on this team?
