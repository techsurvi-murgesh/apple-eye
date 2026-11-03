# 100 Interview Questions — AI-Native Software Engineer (Backend & API), FlytBase

## AI-Native Development & Agentic Coding (1-14)
1. Which AI coding tools do you use daily (Claude Code, Cursor, Codex, Hermes) and what does your workflow look like?
2. How do you write prompts/context so an AI copilot produces correct code in a large unfamiliar codebase?
3. How do you verify AI-generated code before it reaches production?
4. Where does AI-assisted coding help most—greenfield features, refactors, tests, or debugging—and where does it mislead?
5. How do you use AI to debug a failing production issue step by step?
6. How would you build an agentic coding workflow with automated tests and human approval gates?
7. How do you keep an AI copilot from hallucinating APIs or leaking secrets/context?
8. How do you measure the real velocity gain from AI tools on a team?
9. How would you onboard an AI tool into CI (review bot, test generation, changelog)?
10. Describe a time an AI-suggested solution was wrong and how you caught it.
11. How do you keep AI-assisted code consistent with team style and architecture?
12. How do you use AI to accelerate learning a new stack (Go, Kubernetes, React)?
13. What guardrails (linting, type checks, tests, review) make AI velocity safe?
14. How do you decide when not to use AI and just write the code yourself?

## Backend & API Development / Microservices (15-30)
15. Walk through designing a REST API for creating and tracking drone missions.
16. REST vs GraphQL vs gRPC—how do you choose for real-time backend services?
17. How do you design a scalable microservice and where do you draw service boundaries?
18. How do you version an API without breaking existing clients?
19. How do you make an endpoint idempotent so retries are safe?
20. How do you design authentication and authorization (JWT/OAuth) for a multi-tenant API?
21. How do you handle pagination, filtering, and large result sets efficiently?
22. How do you design rate limiting and prevent abuse on public APIs?
23. How do you handle long-running jobs—sync vs async, queues, webhooks?
24. How do you ensure API latency stays low as traffic grows?
25. How do you structure error responses and HTTP status codes consistently?
26. How do you validate input and prevent injection at the API boundary?
27. How would you migrate a monolith to microservices incrementally?
28. How do you handle distributed transactions or eventual consistency across services?
29. How do you document and contract-test APIs (OpenAPI, schema registry)?
30. How do you design a backend service in Go vs Node.js—tradeoffs for this role?

## Data Structures, Algorithms & Concurrency (31-42)
31. Given a stream of telemetry events, how do you compute a rolling average efficiently?
32. How would you design an in-memory cache with TTL and eviction?
33. Explain concurrency in Go: goroutines, channels, mutexes, WaitGroups, context.
34. How do you avoid race conditions and deadlocks in concurrent services?
35. How do you bound concurrency so you don't overwhelm a downstream dependency?
36. How do you process a large batch of jobs in parallel with backpressure?
37. What's the difference between concurrency and parallelism, with a backend example?
38. How would you detect and handle errors in a fan-out/fan-in worker pattern?
39. Design a rate limiter (token bucket) and analyze its complexity.
40. How do you find the top-K most frequent events in a high-volume stream?
41. How do you handle timeouts and cancellation across service calls?
42. When would you choose a queue over direct calls, and how do you size it?

## Distributed Systems & System Design (43-54)
43. Design the backend for a fleet of drones sending real-time telemetry to a dashboard.
44. How do you achieve high availability and fault tolerance in a microservices system?
45. Explain CAP theorem and how it affects your database/service choices.
46. How do you handle partial failures, retries, and circuit breakers?
47. How do you design idempotent consumers for an event-driven pipeline?
48. How do you keep data consistent between services (sagas, outbox pattern)?
49. How do you do service discovery and load balancing between microservices?
50. How do you design for observability: logs, metrics, traces, correlation IDs?
51. How would you scale a real-time system from 10 to 10,000 concurrent clients?
52. How do you handle clock skew and ordering in distributed event streams?
53. How do you plan for multi-region deployment and data residency?
54. How do you set SLOs and reason about error budgets for a live product?

## Cloud & Infra — AWS/GCP/Kubernetes/Docker/CI-CD (55-72)
55. How do you containerize a Python or Node.js backend for production?
56. How do you write a secure, minimal Dockerfile (multi-stage, non-root, pinned)?
57. Explain core Kubernetes objects: Pods, Deployments, Services, Ingress, ConfigMaps, Secrets.
58. How do you deploy, manage, and debug a service on Kubernetes/EKS?
59. How do you debug CrashLoopBackOff, OOMKilled, and Pending pods?
60. How do you configure liveness/readiness probes and resource requests/limits?
61. How does horizontal pod autoscaling work and when do you use it?
62. How do you manage config and secrets across environments on K8s?
63. How do you do zero-downtime rolling updates and safe rollbacks?
64. How do you expose a service externally (Ingress/ALB) and manage TLS?
65. How do you troubleshoot "works in cluster but not from outside"?
66. How do you manage AWS infrastructure as code (Terraform) for a microservice?
67. How do you choose between EC2, ECS, EKS, Lambda, or Cloud Run for a workload?
68. How do you design CI/CD for fast, safe deploys (GitHub Actions)?
69. What quality gates belong in a pipeline (lint, tests, image scan, plan)?
70. How do you manage secrets in CI/CD and avoid leaking credentials?
71. How do you monitor services (Prometheus/Grafana) and alert without noise?
72. How do you control cloud cost while scaling a global deployment?

## Real-Time, Drone & Physical AI Domain (73-82)
73. What does "Physical AI" and drone autonomy mean to you at a systems level?
74. How would you design a low-latency command/control channel between a cloud service and a drone?
75. How do you handle intermittent connectivity and offline buffering for field devices?
76. How would you ingest and store high-frequency telemetry (positions, video metadata)?
77. How do you design geofencing or no-fly-zone validation on the backend?
78. How do you ensure safety-critical commands are authenticated and auditable?
79. How do you handle time-series data and query it for historical playback?
80. How would you stream live drone video status to a web dashboard?
81. How do you design alerts for mission failures or anomalies?
82. How do you collaborate with robotics and AI teams on shared interfaces?

## Full-Stack / Frontend & Dashboards (83-90)
83. How do you build a React dashboard consuming a real-time backend feed?
84. How do you handle WebSockets/SSE on the frontend, including reconnects?
85. How do you keep frontend and backend contracts in sync?
86. How do you optimize frontend performance for large data tables/maps?
87. How do you handle auth/session management in a SPA?
88. How do you approach responsive/accessible UI with limited time?
89. How do you debug a bug that spans frontend, API, and database?
90. What's your approach when you must touch UI but you're backend-heavy?

## Debugging, Production & Velocity (91-96)
91. Walk through debugging a slow API end-to-end (frontend → service → DB).
92. A deploy broke production—how do you triage and roll back fast?
93. How do you balance shipping fast vs maintaining correctness?
94. How do you prototype an idea in a day and then productionize it?
95. How do you write tests that give confidence without slowing delivery?
96. How do you handle on-call and production incidents in a lean team?

## Culture, Ownership & Behavioral (97-100)
97. Describe a time you owned a feature end-to-end and shipped it fast.
98. How do you work across backend, cloud, robotics, and product with no rigid silos?
99. How do you learn a new stack or tool quickly without hand-holding?
100. Why FlytBase, why this AI-native backend role, and what would you ship in your first 90 days?
